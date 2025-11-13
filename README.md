# NVIDIA DGX OS for ASUS Ascent GX10
To download NVIDIA DGX OS for ASUS Ascent GX10, please visit [ASUS Product Support For ASUS Ascent GX10](https://www.asus.com/networking-iot-servers/desktop-ai-supercomputer/ultra-small-ai-supercomputers/asus-ascent-gx10/helpdesk_download?model2Name=ASUS-Ascent-GX10).

## Release Notes
- 7.2.3-3-20251007074705
    - First NVIDIA DGX OS release for ASUS Ascent GX10

## How to install DGX OS for ASUS Ascent GX10 

- Obtaining the DGX OS ISO image for ASUS Ascent GX10 

    - Go to releases site: https://www.asus.com/networking-iot-servers/desktop-ai-supercomputer/ultra-small-ai-supercomputers/asus-ascent-gx10/helpdesk_knowledge?model2Name=ASUS-Ascent-GX10
    - Download the ISO image and save it to your local disk.
    - Uncompress the downloaded file and use the tool such as the md5sum command to print the MD5 hash and compare it with the value for this ISO image to make sure the file integrity. 

- Installing the DGX OS image for ASUS Ascent GX10 
    - Installing the DGX OS Image from a USB Flash
        - After obtaining the DGX OS ISO image for ASUS Ascent GX10, create a bootable installation medium, such as a USB flash drive, that contains the image.
        - On Linux, you can use the dd command. On Windows, you can use software such as Akeo Rufus or balenaEtcher. 
- Booting the DGX OS ISO image for ASUS Ascent GX10: These instructions describe how to boot the DGX OS ISO image for ASUS Ascent GX10 locally. 
    - Plug the USB flash drive containing the OS image into the ASUS Ascent GX10 system. 
    - Connect a monitor and keyboard directly to the ASUS Ascent GX10 system. 
    - Boot the system and then press Del key when the ASUS logo appears to get to the boot menu. 
    - Select the USB volume name that corresponds to the inserted USB flash drive and boot the system from it.
    - Continue to DGX OS ISO Boot Options for ASUS Ascent GX10 for a description of the GRUB menu options and for instructions on completing the installation process. 
- DGX OS ISO Boot Options for ASUS Ascent GX10
    - When the system boots up, select DGX Spark Installation Option from the GRUB menu.
    - Then, select the option Install DGX OS X.Y.Z for DGX Spark and the installation process will start. (Here X.Y.Z is the version.) This will take a while.
    - Once the installation is completed, the device will be rebooted, and you will see the Get Started screen.
    - Please click on the Get Started and follow the instructions to complete the OOBE. You can refer to the following video. 
