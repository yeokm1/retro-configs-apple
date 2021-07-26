# PowerBook G4 A1025 (Titanium) (PowerBook3,5)

This laptop was released in Nov 2002 and is the last of the PowerBook G4 line that can natively boot into Mac OS 9.

This guide will be about installing both Mac OS 9.2.2 and OS X 10.4 Tiger on this system as a dual boot configuration.

## Hardware

* CPU: Single-core 1 GHz PowerPC G4
* Graphics: ATI Radeon 9000 with 64 MB of DDR SDRAM
* RAM: 1GB 2x 512MB PC-133

<img src="images/powerbookg4ti-osx.jpg" width="600">

With OS X Tiger 10.4.

<img src="images/powerbookg4ti-os9.jpg" width="600">

With OS 9.

### Storage Drive

<img src="images/powerbook4gti-ssd.jpg" width="600">

Storage is provided by a 128GB Transcend MSA230S mSATA SSD.

<img src="images/powerbook4gti-msata-ide.jpg" width="600">

The drive is mounted into a mSATA-IDE adapter then inserted into the laptop.

## OS Images

### Mac OS X Tiger 10.4

I used the 5-CD version this as the DVD drive on this PowerBook G4 cannot read DVD+R discs which I have. I don't have DVD-R discs to burn to.

After installation, the OS can be updated to 10.4.11 as Apple's update servers are still active.

https://macintoshgarden.org/apps/mac-osx-mac-os-10-ppc

### Mac OS 9.2.2

For the OS 9.2.2 disk, I opted to use the image from [MacOS9Lives forum](http://macos9lives.com/smforum/index.php/topic,4366.0.html) as they are ISO images and are easier to work with on modern systems.

Since this machine can natively boot into Mac OS 9, I used the [Mac OS 9.2.2 Universal Install](http://macos9lives.com/smforum/index.php/topic,2109.0.html) for the Classic Environment.

## Installation

Here are the high level steps I used to install both operating systems.

1. Boot from Tiger OS disk and partition disk
2. Complete Tiger OS installation and all updates
3. Boot from Mac OS 9 install CD and complete the installation.
5. If Classic Environment is desired, copy OS9 Systems Folder to the OS X partition and setup Classic.

### Mac OS X 10.4 Tiger

#### 1. Boot from the Tiger install CD

#### 2. Once it starts, launch Disk Utility to partition the disk.

<img src="images/powerbookg4ti-partition-os9.jpg" width="600">

OS9 gets the first partition of 40GB.

<img src="images/powerbookg4ti-partition-osx.jpg" width="600">

OSX gets the second partition of about 80GB.

Since this machine natively supports booting into OS 9, the option to install Mac OS 9 drivers is given.

#### 3. Continue with the setup utility to the end

<img src="images/powerbookg4ti-disk-selection.jpg" width="600">

Remember to select the correct disk.

#### 4. Install updates

You may need to run the Software Update tool a few times to finish updating all software.

<img src="images/powerbookg4ti-system-about.jpg" width="600">

Here is a fully updated OS X 10.4.11 Tiger installation.

### Mac OS 9

Once OS X is installed, we can proceed directly to Mac OS 9. 

#### 1. Boot from OS 9 install CD

Boot from the `Mac OS 9.2.2 Universal Install for the Classic Environment` ISO.

<img src="images/powerbookg4ti-select-os9-cd.jpg" width="600">

Press the Option key to get to this boot menu. Select the MacOS9Lives Live CD.

<img src="images/powerbookg4ti-select-os9cd-start.jpg" width="600">

Once selected, it will boot up into a LiveCD environment.

<img src="images/powerbookg4ti-select-os9cd-drive-setup.jpg" width="600">

These applications should start automatically. Close the Drive Setup program as it is not needed.

#### 2. Install to the hard drive

Start Apple Software Restore from the CD.

<img src="images/powerbookg4ti-apple-software-restore.jpg" width="600">

Make sure the correct partition is selected.

<img src="images/powerbookg4ti-apple-software-restoring.jpg" width="600">

#### 3. Start from the native OS 9 boot partition

<img src="images/powerbookg4ti-os9-starting.jpg" width="600">

OS 9 booting up

<img src="images/powerbookg4ti-os9-fresh.png" width="600">

Reached the retro desktop!

## Switching operating systems

### Reboot to OS X from OS 9

Go to Apple Menu -> Control Panels -> Startup disk

<img src="images/powerbookg4ti-os9-select-startup-disk.png" width="600">

Select the Mac OSX disk to boot from.

### Reboot to OS 9 from OS X

Go to System Preferences -> Startup Disk

<img src="images/powerbookg4ti-osx-select-startup-disk.png" width="600">

Since this machine can officially boot to OS 9, OS 9 partition is available as a boot option.

### On machine start

One can press the Option key immediately on machine start.

<img src="images/powerbookg4ti-boot-menu.jpg" width="600">

The boot menu will show the available boot options.

### Mac OS 9 Classic Environment in OS X

The Mac OS 9 System and Application folders have to be copied from the `Mac OS 9.2.2 Universal Install` ISO's internal restore image file `MacOS9Lives.img` to any place of your choosing.

<img src="images/powerbook4gti-classic-files.jpg" width="600">

Here it shows the depth of files needed to be open.

<img src="images/powerbook4gti-classic-running.jpg" width="600">

After that run the `Classic` applet from `System Preferences`. Configure the applet to the location of the OS 9 system files then start it.