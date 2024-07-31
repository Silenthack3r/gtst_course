# Apps
## kali have groups of apps like..
1. Info gathering
	most famous tool- **nmap**
2. Vuln analysis
	mft- **nikito, nmap**
3. Web app analysis 
	mft- **burpsuit**
4. Database Assessment
	mft- **sql map**
5. passwd attacks
	mft-**John the riper, hashcat**
6. Wireless attacks
	mft-**aircrack-ng, wifite, river**
7. reverse engineering
	mft- **apk-tool** 
8. Exploitation Tools
9. Sniffing & Spoofing
	Wireshark
10. Post exploitation
	powersploit
11. Forensics
12. Reporting Tools
	 mft-**recordmydesktop**
13. Social Engineering Tools
# Linux Commands
- The terminal have 5 parts
	- Username=name given when opening 
	- Hostname=name of machine
	- Current dir=PATH, folder(usually ~ tida)
	- Privilage=$-user # -root
	- Command place= the space after $ sign
- Home directory is  ~
- Local directory with .
- All directory *
## Linux Command Basics
- All commands have options and arguments 
Commands are **small programs that do one task well.** 
1. ls command
	lists info about the files in the directory we are in.
	- ls -l
		detailed list
	- ls -a
		list hidden files
	- ls filename
		
	- ls -R
		lists the dirs and file in all dirs 

2. cd 
	cd/= 
3. pwd
4. echo
	- > means save
	- >> to save to an existing file/append
5. cat
	shows content of file
6. head
	shows only first line
7. tail
	shows only lastline
8. less
	shows all content
9. touch
	 creates any kind of files
10. mkdir
	makes dirs
11. clears
	clears up the screen
12. rm
	used to remove dirs
	you have to use options
	rm-rf
13. cp & mv
	cp-copy dirs, files
	mv-move dirs, files
14. grep
15. wc
## multiple command execution
1. &&(and)
	 on && operation all commands you entered will be executed  if both are working with out error. is there is one wrong command it will not work.
2. || (or)
	on || operation all commands you entered will be executed wether both are working or oone is working no need for both to work.
3. | (piping)
	on | will help you run commands by using the output of the 1st command as the input for the next one.