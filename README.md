# New firmware released by NVIDIA enhances system stability
A recent software update has been released by Nvidia, and all users will be prompted to install the update when they first power on their devices and complete the initial setup.
•   The update is mandatory for all GB10 devices from all vendors.
•   The update includes firmware, OS components and drivers. The update process may take approximately 30 to 40 minutes, depending on the user's internet connection speed.

Update the latest firmware version
Please follow the SOP for updating the firmware:
a.	To access the BIOS main page, turn on the GX10 and press the Del button. 
b.	Go to Advance and set up Power On Behavior to Auto Boot by pressing the Enter button. 
Note: After the setup, the system may need to reboot several times into Ubuntu.

<img width="840" height="383" alt="image" src="https://github.com/user-attachments/assets/74d170a9-fd42-40eb-bf25-12eb1017fe96" />








There are two methods to update the firmware: online and offline: 

a.	Online Firmware Update
We strongly recommend using the DGX Dashboard for all system updates on your ASUS Ascent GX10. The dashboard ensures your system stays up to date with the latest NVIDIA-optimized components and configurations. While standard Ubuntu package management methods will work, the dashboard provides the most reliable and tested update path for your DGX system.


Using DGX Dashboard for Updates
The DGX Dashboard is the primary and recommended way to perform system updates on your ASUS Ascent GX10. It provides a centralized interface for:
•	Viewing available system updates
•	Installing security patches and system updates
•	Managing NVIDIA driver updates
•	Managing firmware updates
•	Monitoring update status and progress
For detailed information about using the DGX Dashboard, including how to access it and perform updates, see DGX Dashboard.
Warning
Before performing any system or firmware updates:
•	Ensure your system is connected to a stable power source
•	Close all running applications and save your work
•	Have a recovery plan in place
•	Schedule updates during maintenance windows when possible

Manual System Updates
Note: While manual updates using standard Ubuntu package management commands will work, we strongly recommend using the DGX Dashboard for all updates to ensure optimal system performance and compatibility.
For advanced users or when the DGX Dashboard is not available, you can perform system updates manually using the following steps:
1.	Open a remote or local terminal on the ASUS Ascent GX10 device.
2.	Run the following commands:
sudo apt update
sudo apt dist-upgrade
sudo fwupdmgr refresh
sudo fwupdmgr upgrade
sudo reboot


These commands will:
•	Update the package lists and upgrade all installed packages (including OS components and drivers)
•	Refresh the firmware metadata and upgrade all firmware components
•	Reboot the system to apply updates

b.	Offline update instructions
1.	Visit the ASUS Support website and download capsule_update.sh and fw.cap from the ASUS official website.
Update the latest firmware
BIOS: 0101 (bsp_v11_socfw302_bios_0101_ec_2.66.3.3_signed.cap)
EC: 2.66.3.3 (ec_2.66.3.3_signed.cap)
2.	Transfer the firmware files to the system SSD.
3.	Open the Terminal and navigate to the folder containing the firmware.
4.	Set file permissions with the command:

chmod -R 777 *
5.	Execute the update script:

./capsule_update.sh fw.cap
6.	The system will automatically reboot and complete the firmware update process.

Note: We strongly advise using the DGX Dashboard for all system upgrades online on your ASUS Ascent GX10 to ensure that your system is running the most recent firmware.
process. 
- DGX OS ISO Boot Options for ASUS Ascent GX10
    - When the system boots up, select DGX Spark Installation Option from the GRUB menu.
    - Then, select the option Install DGX OS X.Y.Z for DGX Spark and the installation process will start. (Here X.Y.Z is the version.) This will take a while.
    - Once the installation is completed, the device will be rebooted, and you will see the Get Started screen.
    - Please click on the Get Started and follow the instructions to complete the OOBE. You can refer to the following video. 
