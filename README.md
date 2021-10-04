# Gentoo-Install-Scripts
An install script to automate setting up a base gentoo system. Note: An ncurses based ui, or a gtk based GUI will be coming.

# Usage
Download a stage3 tarball from gentoo's website, and place it in the stage3 folder. Boot the gentoo live cd, and clone this repository in the live cd. Then create your partitions, and run the script. 

# Important 
By default the script uses the default partition table in the gentoo handbook

Filesystem<br />
`/dev/nvme0n1p1 ->` BIOS boot partition<br />
`/dev/nvme0n1p2 ->` Boot partition<br />
`/dev/nvme0n1p3 ->` Swap partition<br />
`/dev/nvme0n1p4 ->` Root partition<br />
 
This script will need some modifications especially the kernel config file. These modifications depend on your system. Also this script uses openrc as its primary init system. Also the script at this point in time doesn't automatically download a stage3 tarball you will have to do that your self and place it in the stage3 folder.

Another thing to note is that the script by default builds for UEFI systems. This can easily be changed

