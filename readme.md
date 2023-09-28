# Fix black screen on startup: IOReg 
https://dortania.github.io/OpenCore-Post-Install/gpu-patching/intel-patching/connector.html

framebuffer-patch-enable = 01000000
Enables WhateverGreen's patching mechanism
framebuffer-conX-enable = 01000000
Enables WhateverGreen's patching on conX
framebuffer-conX-type = 00080000
Sets the port to HDMI(<00 08 00 00>)

# Fix boot loop
Set secure boot disabled

# for EFI in hard drive, must change file/dir name
EFI
|-MICROSOFT
|    |-BOOT
|       |-BOOTMGFW.EFI 
|-OC
  |- ACPI
  ...

# Sonoma
- Update WhateverGreen, Lilu, VirtualSMC, AppleALC, Bluetooth, Airportltlwm
- Fix DisplayPort for HDMI port 1: https://lzhoang2601.github.io/post-install/gpu/intel-igpu#hdmi-sound
- Add WhateverGreen's patch to boot-args