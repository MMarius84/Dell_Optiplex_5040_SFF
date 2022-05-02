# Dell_Optiplex_5040_SFF

This is a EFI for MacOS based on the OpenCore project.
This EFI is created to run on the DELL Optiplex 5040SFF, other Dell machines and variants may be able to run it.

The EFI/Config is set to utilize the iGPU, any other GPUs used will need to have the config adjusted.

PC Spesc:

CPU:    I5-6500
GPU:    Intel HD 530 (iGPU)
RAM:    4Gb DDR3L - 1600 Mhz

!!!!!!!!  IMPORTANT   !!!!!!!!!!

For MacOS to be installed two major keypoints must be addressed:
1. MSR needs to be deactivated - Not available in BIOS nor is it addressible from the config.plist
2. (DVMT) Graphics Memory allocation needs to be more than 32Mb, otherwise installer/OS will boot to a black screen
-> the above changes can be done only by changing the values within the BIOS (BIOS Modding) which may lead to a BRICKED MACHINE

!!!!!!!!  IMPORTANT   !!!!!!!!!!
