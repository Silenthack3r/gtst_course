# Linux File Hierarchy 
- Linux/UNIX have special file system than windows.
- File system is a directory structure that the OS uses.
## System Files
- System Files are files used by the system software(OS),
- Windows: system files appear under the **Local disk c**.
- Linux: System files appear under the **root directory (/).**
1. /(root)
 - every single file and directory starts from the root directory.
 - The only root user has the right to write under this directory
 - /root is the root  user's home directory, which is not the same as /.
 2. /boot- boot loader files
	 - Kernel initrd, vmlinux, grub files are located under /boot
	 - E.g.:
		 initrd.img-2.6.32-24-generic, vmlinux-2.6.32-24-generic
3. /dev-essential Device Files
	- These include terminal devices, usb, or any device attached to the system.
	- E.g.:
		/dev/tty1, /dev/usbmon0
	to create user on kali 
	sudo mkdir /home/username