# Some advanced user commands
- To change password of user
	- sudo passwd username
- To change user id
	- sudo usermod -u new_id username
- To delete user
	- sudo userdel -r username
- To change users on terminal
	- su username
# Sudoers file
- The sudoers file is a file **Linux and Unix administrators use to allocate aystem rights to system users** 
- The user you created doesn't have power to use **sudo** as the original
<!-- not finished -->
- To make users use sudo use -sudo visudo
# Linux File Permisssion
- Every file on linux have their own 
	- Owner
	- permissions
- There are 5 main parts on the listing
- Permission
- Owners
- Date
- Size
- filename
## Ownership
- ownership is the owner of the file
- This have 2 kinds
	- User
	- Group
- To change the owner of file you can use the command
	- sudo chown user:group filename
- question: when trans the ownership what is the use of changing the group.
## Permission
- there are 3 types of permissions
	- read(r)
	- Write(w)
	- Execute(x)
- The folders and files differ with the 'd' for folder and '-' for dir(folder)
- There still the permission have three parts.
	- user-group-other
- User (u) => Power of user defined on the ownership
- Group(g) => power of group defined on the ownership
- other(o) =>power of other users
- All(a) => power of all which can be found in the 3 above owners
- command to change permission of file
	- sudo chmod - or + option(like r,x,w) filename
### chmod comamnd
- this command helps to change file permission
- Each of the permission have a no. representations
- <!--not finished--> 
	- 4=> r
	- 2=> w
	- 1=> x
- The parameter can bem in numbers and symbols
1. parameters in symbol
	 -  chmod a+x filename -> adding permission for all (chmod +x filename)
	 - chmod u+x filename -> adding execute permission for user
	 - chmod g+x filename -> adding permission for group
	 - chmod o+x filename -> for other
	 - chmod -x filename -> removing execute from all
 2. parameters in no.
	 - chmod -621 filename -> 6.for user, 2. for group, 1. for other (6=4+2). 6=rw
	 - chmod -777 filename-> 7for user 7 for group 7 for others(7=4+2+1), 7=rwx
### Special file permissions
-there area nother 3 special permissions, you may encounter on your pentest journey
-they are
 - SUID bist(s)-set user-set user ID bit-add 4 infront of our numeric value -> 4000
 - SGID bits(S)-set group ID bit-add 2 infront of our numeric value-2777
 - sticky bits(t)-set other ID bit-add 1 infront of our numeric value->1602
-They are permissions like x. but they will set the x permission to the user who settled them.
-E.g.:if mr.A add suid bit to a program taht program taht program will be executed with permission of mr.A
	-meaning if admin add suid bit on some program. then any user if they got that program they can run it as with any sudo password.
## package installation on linux
- On linux to install softwares you use package managers
	- E.g.: apt,packman,pkg
- package managers are a **free software user interface that work with an online server to handle the installation ang removal of software on Debian, and Debian based Linux distributions.** 
## The repository
This is the site/server kali use to upload the packages.
## advanced package tool /apt/
- apt is a free software user interface that work with an online server to handle the installation ang removal of software on Debian based linux.
- the old 'apt' used as 'apt-get'
- syntax
	- sudo apt update(update)
	- sudo apt search softwarename(search)
	- sudo apt remove software (remove the tool only with out the files)
	- sudo apt upgrade(shows upgradable)
	- sudo apt purge softwarename(completely delete with files)
## package depemdemcies
- A software can be built based on another program called 'modules'
- so,  a program to work properly, the dependencies have to be installed successfully
- Those package managers install the software+dependencies.

	