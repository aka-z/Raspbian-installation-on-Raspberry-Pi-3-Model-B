# Raspbian-installation-on-Raspberry-Pi-3-Model-B
 *Raspbian Jessie with Pixel*
 
# REFERENCE

http://www.pyimagesearch.com/2016/04/18/install-guide-raspberry-pi-3-raspbian-jessie-opencv-3/

# INTRODUCTION

The Raspberry Pi 3 is the third-generation Raspberry Pi. It replaced the Raspberry Pi 2 Model B in February 2016. This latest model (Raspberry Pi 3) includes 802.11n WiFi, Bluetooth 4.0, and a quad-core 64-bit ARM Cortex A53 running at 1.2 GHz. It’s a usable desktop computer. 

And the goal of this manual is to thus guide you step-by-step through the compile and installation process. There are ten parts in this document. If you follow these steps, you can operate image processing using OpenCV on the Raspberry Pi 3 Model B. Anyway, let’s go ahead and get started installing OpenCV 3 on your brand-new Raspberry Pi 3 running Raspbian Jessie.

# VERSION INFO
- __Raspberry Pi3 Model B__：Raspbian JESSIE WITH PIXEL

  Image with PIXEL desktop based on Debian Jessie
 
  Version：January 2017
 
  Release date：2017-01-11
 
  Kernel version：4.4
 
- __OpenCV__：3.1.0
- __Python__：3.4



# Raspbian Installation Step
- __Windows(Recommend)__:

   - __Step1__： Download the “SD Card formatter” from the URL below 
  
       https://www.sdcard.org/cht/downloads/formatter_4/
       
   - __Step2__： Download the Win32DiskImager utility from the Sourceforge Project page as a zip file; you can run this from a USB drive.
  
       https://sourceforge.net/projects/win32diskimager/

   - __Step3__：Extract the executable from the zip file and run the Win32DiskImager utility; you may need to run this as administrator. Right-click on the file, and select Run as administrator.
  
   - __Step4__： Select the image file you extracted earlier.
 
   - __Step5__：Select the drive letter of the SD card in the device box. Be careful to select the correct drive; if you get the wrong one you can destroy the data on your computer's hard disk! If you are using an SD card slot in your computer and can't see the drive in the Win32DiskImager window, try using an external SD adapter.
  
   - __Step6__：Click Write and wait for the write to complete.
  
   - __Step7__：Exit the imager and eject the SD card.


- __Mac(Not Recommend)__:

  Please refer the information from the URL below：
  
  https://www.raspberrypi.org/documentation/installation/installing-images/mac.md

- __Linuux__:

  Please refer the information from the URL below：
  
  https://www.raspberrypi.org/documentation/installation/installing-images/linux.md

# OpenCV Installation Step
- __Step 1__ : Expand filesystem

	The prepared images for the Raspberry Pi are created for SD cards of the size of 2GB. The SD card can be resized or restructured to use the full size of a SD card that is greater than 2GB.
	```
 	$ sudo raspi-config
	$ sudo reboot
	$ df –h
 	```
	And you’ll see Raspbian filesystem has been expanded to include all 8GB of the micro-SD card.

	Filesystem     	 	Size  	Used 	Avail 	Use% 	Mounted on
	
	/dev/root       		7.2G  	3.3G  	3.6G  	48%	/
	
	devtmpfs        		459M        0  	459M   	 0% 	/dev
	
	tmpfs           		463M        0  	463M  	 0% 	/dev/shm
	
	tmpfs           		463M  	6.4M  	457M   	 2%	/run
	
	tmpfs           		5.0M  	4.0K  	5.0M   	 1%	/run/lock
	
	tmpfs           		463M        0  	463M   	 0% 	/sys/fs/cgroup
	
	/dev/mmcblk0p1  	60M   	20M   	41M  	34% 	/boot
	
	tmpfs            		93M     	   0   	93M   	 0%	/run/user/1000

	OpenCV, along with all its dependencies, will need a few gigabytes during the compile, so you should delete the Wolfram engine to free up some space on your Raspberry Pi 3:
	`$sudo apt-get purge wolfram-engine`


- __Step 2__ : Expand filesystem
- __Step 3__ : Expand filesystem
- __Step 4__ : Expand filesystem
- __Step 5__ : Expand filesystem
- __Step 6__ : Expand filesystem
- __Step 7__ : Expand filesystem
