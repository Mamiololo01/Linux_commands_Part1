# Linux_Overview
Overview of Linux commands.

Basic Linux commands PART 1

Check Free CPU memory
Free; This shows the used, total and free memory.



Check current processes
Ps; shows a snapshot of current processes.

 


Check active Linux processes
top; displays current Linux processes.
htop: gives graphical representation.
 


IP traffic monitor
Iptraf; shows a GUI page for ethernet traffic 
 

Iptraf -ng nc; captures traffic
 

Controlling Network manager
Nmcli; shows all network interface
 

List files and directories
ls; list all files and directories
ls -a; list all hidden files
ls-al;
ls -ah;
 

 

Controls the hostname
hostnamectl; displays all info on controlling the hostname
 

Netstat
Check listening ports
netstat -tulpn; shows all active ports on ‘’listening’’ mode

Check all open ports
netstat
 

Make directory
mkdir; creates a directory
 

Check present working directory
pwd; checks the current working directory
 

Remove files and directory
rm filename ; removes a file
rm -r directory_name; removes a directory
 

To check uptime
uptime; to check uptime of the server.
 

Copy file content
 cp {filename1} {filename2}; copies the content of one file to another
 

Displays content of file
cat {file_name}; displays content of {file_name}

Create a new file
touch {file_name}; creates a new file
 

File {filename}; shows the type of document
 

Removes files or directory
rm -I {file_name}; ask for permission before removing a file
rm -rf {file_name}; forcefully removes a file or directory
rm {file_name}; removes only a file, not the file_name.

More
more is a filter for paging through text one screenful at a time. This version is especially primitive. Users should realize that less (1) provides more(1) emulation plus extensive enhancements.

head {file_name}; shows the first 10 lines in the file.
tail {file_name}; shows the last 10 lines in the file.

Displays active users
id; displays active users 
 

Shows system logins
last; shows lists of all active system logins
 

Current logon
who; shows who is currently logged in.
 


Add new group
groupadd {group_name}; adds a new group.
 

Add a new user
adduser {user_name}; creates a new user.
 

Delete user
userdel {user_name}; deletes an active user.
 

Modify user
usermod {user_name}; modifies an active user.


Change directory group
chgrp {group_name} {directory_name}; changes the directory group.

Install package manager
sudo apt install {package_manager};  installs package manager.
 

Terminate a Linux process
Kill {PID}; Kills a Linux process under a given ID.

Terminate all processes
Kill all {process_name}; Terminates all processes with the labelled ID

Resume stopped jobs
bg; list and resume stopped jobs in the background
 

Resume recently suspended jobs
fg; brings up the most recently suspended jobs to the foreground.
 

Shows kernel info
Uname -a; displays kernel release info
 

Display current date
date; shows current time.
 

Displays IP address
hostname -I; shows IP address
 

List IP address
Ip add show; list all IP address and network interfaces
 

Add IP address to interface.
ip address add {IP_address}; assigns IP address to interface etho

Shutdown
Shutdown {hh:mm}; schedules shutdown
Shutdown now; immediate shutdown

DISKS
df -h; shows free and used space on mounted system
 
df -ah; shows disk usage for all files and directory.
 

SSH
ssh user@host; connects to host as user
ssh -p {port} user@host; connect to host using a specific port number

File ownership
Chmod 777 {file_name}; assigns read, write and execute permissions to everyone
Chmod 755 {file_name}; assigns read, write, and execute to owners, read and execute to group and others.
Chmod 766 {file_name}; assigns full ownership to owner, read and right permission to group and others.
Chmod 600 {file_name};  full permission to owner, no access to group and others.
Chown {user_name}:{group} {file_name}; changes the owner and group membership of a file.

DNS information
Dig; shows dns information about a domain
 

NSLOOKUP
nslookup {domain_name}; displays info about internet domain.


Download file from internet
wget {filename/web address}; downloads the file or the document from webpage
 

Remote file save
Curl -o {file_name}; saves a remote file to your system

Lock account
Usermod -L {account_name}; locks an account.

Admin user add.
sudo useradd -m {user_name}; adds users as admin

Set password
Sudo password {user_name}; sets user password.

Query system
Journalctl; queries the system 
 

SYSTEMCTL
Controls the systemd system and service manager
Manage service
Service {service_name} status
Systemctl status {service_name}
Systemctl status httpd.service; checks status of httpd service
Systemctl start httpd. service; starts httpd service
Systemctl restart httpd. service; restarts httpd service
Systemctl status apache2; checks status of apache service

Search files
Ps aux | grep {service_name}; Searches for a pattern in each file.

Disk
Mount; Checking existing mount
 

Ls/mnt



