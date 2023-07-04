# Cyberops-associate
Notas del curso Cyberops Associate

## The Danger

## Fighters in the war against cybercrime

## The Windows operating system

## Linux overview

### 4.1 Linux Basics

### 4.2 Working with the Linux shell
Fabrice Bellard has created JSLinux which allows an emulated version of Linux to run in a browser. [JSLinux](https://bellard.org/jslinux/)
+ Basic commands:
  + mv
  + chmod
  + chown
  + dd
  + pwd
  + ps
  + su
  + sudo
  + grep
  + ifconfig
  + apt-get
  + iwconfig
  + shutdown
  + passwd
  + cat
  + man
+ File and directory commands
  + ls
  + cd
  + mkdir
  + cp
  + mv
  + rm
  + grep
  + cat
 

> In Linux, everything is treated as a file. This includes the memory, the disks, the monitor, and the directories. For example, from the operating system standpoint, showing information on the display means to write to the file that represents the display device. It should be no surprise that the computer itself is configured through files. Known as configuration files, they are usually text files used to store adjustments and settings for specific applications or services. Practically everything in Linux relies on configuration files to work. Some services have not one, but several configuration files.

:computer: LAB - [Working with Text Files in the CLI](https://github.com/13sauca13/Cyberops-associate/blob/5ca05d054f166ffd4dbb1c2012d1aa40390bc565/4.%20Linux%20overview/4.2.6%20Lab_Working%20with%20text%20files%20in%20the%20cli.pdf)

:computer: LAB - [Getting Familiar with the Linux Shell](https://github.com/13sauca13/Cyberops-associate/blob/5ca05d054f166ffd4dbb1c2012d1aa40390bc565/4.%20Linux%20overview/4.2.7%20Lab_Getting%20familiar%20with%20the%20linux%20shell.pdf)

### 4.3 Linux Servers and Clients
For communications we are all time using **IP+Port=Socket** so clients can access server's resources.
+ Usual well-known ports
  + TFTP *69*
  + FTP *20/21*
  + SFTP *22*
  + SSH *22*
  + Telnet *23*
  + DNS *53*
  + DHCP *67/68*
  + HTTP *80*
  + HTTPS *443*
  + POP3 *110*
  + NTP *123*
  + IMAP *143*
  + SNMP *161/162*
 
  :computer: LAB - [Linux servers](https://github.com/13sauca13/Cyberops-associate/blob/45154c5fe8019aab10919e03edcba705fff72c43/4.%20Linux%20overview/4.3.4%20Lab_Linux%20servers.pdf)

Services are managed using configuration files. When the service starts, it looks for its configuration files, loads them into memory, and adjusts itself according to the settings in the files. Configuration file modifications often require restarting the service before the changes take effect.

The following are basic best practices for device hardening.
+ Ensure physical security
+ Minimize installed packages
+ Disable unused services
+ Use SSH and disable the root account login over SSH
+ Keep the system updated
+ Disable USB auto-detection
+ Enforce strong passwords
+ Force periodic password changes
+ Keep users from re-using old passwords
