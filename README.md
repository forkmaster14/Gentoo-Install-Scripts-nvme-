# Gentoo-Install-Scripts
An install script to automate setting up a base gentoo system.

# Usage

1. Clone this repository into the installation media of your choice.
2. Download a stage3 tarball from Gentoo's website, and place it in the stage3 folder.
3. Partition the disks as listed below
4. Create the "/mnt/gentoo" directory (If not using Gentoo install media)
4. run the script and follow the instructions.

# Important 
By default the script uses the default partition table in the gentoo handbook

Filesystem<br />
`/dev/(your disk name)1 ->` BIOS boot partition<br />
`/dev/(your disk name)2 ->` Boot partition<br />
`/dev/(your disk name)3 ->` Swap partition<br />
`/dev/(your disk name)4 ->` Root partition<br />
 
This script will need some modifications especially the kernel config file. These modifications depend on your system. Also this script uses openrc as its primary init system. Also the script at this point in time doesn't automatically download a stage3 tarball you will have to do that your self and place it in the stage3 folder.

Another thing to note is that the script by default builds for UEFI systems. This can easily be changed

Note:

The script uses the default Arch linux kernel config. After installation you should change the kernel to your liking.

If you have any issues, create a github issue.
