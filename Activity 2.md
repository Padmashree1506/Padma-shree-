Activity 2

ubuntu@ubuntu:~

man tree -a
Description: All  files  are printed.By default tree does not print
              hidden files.
tree -a
.
├── .arduino15
│   └── preferences.txt
├── .bash_history
├── .bash_logout
├── .bashrc
├── .cache
Remarks: Usefull to see  hidden files.

man tree -d
Description: List directories only.
tree -d
.
├── Arduino
│   └── libraries
├── Desktop
├── Documents
├── Downloads
├── Music
├── My File.txt
├── Pictures
├── Public
├── Templates
├── Videos
└── snap
Remarks: helps to quikly understand the directory hierarchy.

man tree -u
Descripton: Print the username, or UID # if no  username  is  avail‐
              able, of the file.
tree -u
[ubuntu  ]  .
├── [ubuntu  ]  Arduino
│   └── [ubuntu  ]  libraries
│       └── [ubuntu  ]  readme.txt
├── [ubuntu  ]  Desktop
│   └── [ubuntu  ]  ubuntu-desktop-bootstrap_ubuntu-desktop-bootstrap.desktop
Remarks: Helps system admins quikly see if some files are owned by root 
          while others by normal users.

man tree -p
Description: Print  the  file  type and permissions for each file.
tree -p
drwxr-x---]  .
├── [drwxrwxr-x]  Arduino
│   └── [drwxrwxr-x]  libraries
│       └── [-rw-rw-r--]  readme.txt
├── [drwxr-xr-x]  Desktop
│   └── [-rwxr-xr-x]  ubuntu-desktop-bootstrap_ubuntu-desktop-bootstrap.desktop
Remarks: It focuses on permission.


ifconfig
Description: configure a network interface
enp0s3: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
Remark: ifconfig shows network details such as IP address,subnet mask.MAC address
        and packet statistics.
        
ping
Description:send ICMP ECHO_REQUEST to network hosts
ping -c 2 chrome.com
PING chrome.com (216.239.32.27) 56(84) bytes of data.
Remark: If replies are received ,the host is reachable and network is working.

traceroute
Decription:print the route packets trace to network host
Traceroute chrome.com
traceroute to chrome.com (216.239.32.27), 30 hops max, 60 byte packets
1  _gateway (10.0.2.2)  2.968 ms  2.836 ms  2.796 ms
2  _gateway (10.0.2.2)  10.311 ms  10.176 ms  10.055 ms
Remark: Shows the path taken by packets to reach a destination host.

nmap
Description:Network exploration tool and security / port scanner
nmap chrome.com
Nmap scan report for chrome.com (216.239.32.27)
PORT    STATE SERVICE
80/tcp  open  http
443/tcp open  https
Remark: Very useful for security auditing , you can see what attackers might find.

mkdir
Description:make directories
mkdir newfolder
Remark: Makes an empty directory.




