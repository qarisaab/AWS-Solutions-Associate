
#### The linux boot process
After the computer starts the BIOS on the computer checks all the I/O devices and hardware devices once everything is ok the computer can boot.

#### GRUB
The boot program called the GRand Unified Boot loader is the program on most linux distros will look for the section on the hard drive that contains the data needed for the computer to boot an OS. The boot loader than load the linux kernel and then the linux kernel will load the intial RAM disk that contains a bunch of device drivers and start to load the computers drivers that mount the filesystem from the hard disk.

#### Bootlogs
These are the volatile logs that are generated when the computer itself is booted and are volatile. These logs are generated from an area called as kernel ring buffer that is an area of RAM that the kernel writes it system msg to. 
dmesg is used to view the kernel ring buffer. 
jouranlctl -k is used to view the kernel ring buffer.

#### GRUB ON MBR
When the computer is booted the BIOS checks all the hardware devices than load the bootloader the GRUB bootloader is a small 512 byte file that is called as boot.img which is the first 512 bytes of the hard disk and this is the space that is going to be marked with the boot flag. It is called as the stage one of the boot process. The whole purpose of the boot.img file is to locate the core.img file and load it the core.img file is the file that is core.img file exist with an empty space towards the start of the boot disk and this also called as stage 1.5 of the grub boot process. The job of the core.img file is to locate the actual boot partition of the system and in the stage 2 it is where the actual boot partition gets read on the system the grub is looking for a grub.conf or menu.lst file. The other file that is necessary  is called the device.map file that indicate which drive contains the actual kernel and the OS that needs to be booted. Once the file is read than the linux kernel is loaded by the grub and the rest of system is booted up.

