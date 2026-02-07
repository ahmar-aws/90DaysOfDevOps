Process management
1.	ps -U root -u root
Display all processes running under the account root.
2.	 -eo pid,user,command
Display only the columns pid, user and command in ps output
3.	top
Display sorted information about processes
4.	&
Add this character to the end of a command/process to run it in the background
5.	kill PID
Kill a process specified by its process ID PID, which you obtain using the ps command
6.	lsof -u root
List all files on the system opened by the root user. As the output can be long, you may use `lsof -u root
7.	mpstat 1
Display processor-related statistics, updated every second (hence the 1, whereas mpstat 2 refreshes the output every 2 seconds)

File system
1.	Ls
List the names of files and subfolders the current directory. Options include -l, - a, -t which you may combine, e.g., -alt.
2.	ls -l
Also show details of each item displayed, such as user permissions and the time/date when the item was last modified
3.	ls -a
             	Also display hidden files/folders. May combined with ls -l to form ls -al.
4.	Cd
         	 To the $HOME directory
5.	cd ..
Up one level to enclosing folder or parent directory
6.	cd /etc 
To the /etc directory
7.	cmp A B
Compare two files A and B for samenes No output if A and B are identical, outputs character and line number otherwise.
Networking troubleshooting
1.	Ifconfig
Display all network interfaces with IP addresses
2.	ping host
Send ICMP echo request to host, which may be a symbolic name, domain name or IP address
3.	netstat -nutlp
Show listening TCP and UDP ports and corresponding programs
4.	whois domain
Display whois information for domain
5.	dig domain
Display DNS information for domain
6.	wget <LINK>
Download from location LINK


               


