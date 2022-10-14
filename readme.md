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

