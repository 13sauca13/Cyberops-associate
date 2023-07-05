# Cyberops-associate

## 1. The Danger

### 1.1 War stories
:computer: LAB - [Installing the Virtual Machines](https://github.com/13sauca13/Cyberops-associate/blob/d12192f28574fa7a56a9b230b7290bb7acc8e2ad/Resources/Labs/1.1.5%20Lab_Installing%20the%20virtual%20machines.pdf)

:memo: LAB - [Cybersecurity Case Studies](https://github.com/13sauca13/Cyberops-associate/blob/48879fb65d4482c2b97de8945f559186aadb28aa/1.%20The%20Danger/1.1.6%20Lab_Cybersecurity%20case%20studies.pdf)

### 1.2 Threat Actors
Threat actors are individuals or groups of individuals who perform cyberattacks.
+ Amateurs (Script Kiddies)
+ Hacktivist
+ Financial Gain
+ Trade secrets and global politics

:memo: LAB - [Learning the details of attacks](https://github.com/13sauca13/Cyberops-associate/blob/273d62bb4bb4cb75ab18bfca48f4124c31b55ef0/1.%20The%20Danger/1.2.3%20Lab_Learning%20the%20Details%20of%20Attacks.pdf)

### 1.3 Threat impact
Personally identifiable information (PII) is any information that can be used to positively identify an individual.
Two subsets of PII are:
+ PHI (*Personal Health Information*)
+ PSI (*Personal Security Information*)

:memo: LAB - [Visualizing the black hats](https://github.com/13sauca13/Cyberops-associate/blob/6566e92e7b5ff70cf89d64a93a9bd8681dd13df7/1.%20The%20Danger/1.3.4%20Lab_Visualizing%20the%20Black%20Hats.pdf)

## 2. Fighters in the war against cybercrime

### 2.1 The modern Security Operations Center
SOCs provide a broad range of services, from monitoring and management, to comprehensive threat solutions and hosted security that can be customized to meet customer needs. SOCs can be wholly in-house, owned and operated by a business, or elements of a SOC can be contracted out to security vendors.

Elements of a SOC:
+ People
  + Tier 1 Alert Analyst
  + Tier 2 Incident Responder
  + Tier 3 Threat Hunter
  + SOC Manager
+ Process : If a ticket cannot be resolved, the Cybersecurity Analyst will forward the ticket to a Tier 2 Incident Responder for deeper investigation and remediation. If the Incident Responder cannot resolve the ticket, it will be forwarded it to Tier 3 personnel with in-depth knowledge and threat hunting skills.
+ Technoligies
  + SIEM (*Security Information Event Management system*): Used for collecting and filtering data, detecting and classifying threats, and analyzing and investigating threats.
  + SOAR (*Security Orchestration Automation and Response*): Often paired with SIEMs as they have capabilities that complement each other. Similar to SIEMs but they also integrate threat intelligence and automating incident investigation and response workflows based on playbooks developed by the security team.
 
| SOC Metrics | |
| --- | --- |
| Dwell Time | Time that threat actors have access to a network before they are detected, and their access is stopped. |
| MTTD | Mean Time To Detect |
| MTTR | Mean Time To Respond |
| MTTC | Mean Time To Contain |
| Time To Control | Time required to stop the spread of malware in the network. |

## 3. The Windows operating system

## 4. Linux overview

### 4.1 Linux Basics

### 4.2 Working with the Linux shell
Fabrice Bellard has created JSLinux which allows an emulated version of Linux to run in a browser. [JSLinux](https://bellard.org/jslinux/)
+ Basic commands:
  
| Command | Description |
| --- | --- |
| `mv` | |
| `chmod` | |
| `chown` | |
| `dd` | |
| `pwd` | |
| `ps` | |
| `su` | |
| `sudo` | |
| `grep` | |
| `ifconfig` | |
| `apt-get` | |
| `iwconfig` | |
| `shutdown` | |
| `passwd` | |
| `cat` | |
| `man` | |

+ File and directory commands
  
| Command | Description |
| --- | --- |
| `ls` | |
| `cd` | |
| `mkdir` | |
| `cp` | |
| `mv` | |
| `rm` | |
| `grep` | |
| `cat`| |
 

> In Linux, everything is treated as a file. This includes the memory, the disks, the monitor, and the directories. For example, from the operating system standpoint, showing information on the display means to write to the file that represents the display device. It should be no surprise that the computer itself is configured through files. Known as configuration files, they are usually text files used to store adjustments and settings for specific applications or services. Practically everything in Linux relies on configuration files to work. Some services have not one, but several configuration files.

:computer: LAB - [Working with Text Files in the CLI](https://github.com/13sauca13/Cyberops-associate/blob/5ca05d054f166ffd4dbb1c2012d1aa40390bc565/4.%20Linux%20overview/4.2.6%20Lab_Working%20with%20text%20files%20in%20the%20cli.pdf)

:computer: LAB - [Getting Familiar with the Linux Shell](https://github.com/13sauca13/Cyberops-associate/blob/5ca05d054f166ffd4dbb1c2012d1aa40390bc565/4.%20Linux%20overview/4.2.7%20Lab_Getting%20familiar%20with%20the%20linux%20shell.pdf)

### 4.3 Linux Servers and Clients
For communications we are all time using **IP+Port=Socket** so clients can access server's resources.
| Service | Port |
| --- | --- |
| TFTP | *69* |
| FTP | *20/21* |
| SFTP | *22* |
| SSH | *22* |
| Telnet | *23* |
| DNS | *53* |
| DHCP | *67/68* |
| HTTP | *80* |
| HTTPS | *443* |
| POP3 | *110* |
| NTP | *123* |
| IMAP | *143* |
| SNMP | *161/162* |
 
  :computer: LAB - [Linux servers](https://github.com/13sauca13/Cyberops-associate/blob/45154c5fe8019aab10919e03edcba705fff72c43/4.%20Linux%20overview/4.3.4%20Lab_Linux%20servers.pdf)

### 4.4 Basic Server Administration
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

Log files are the records that a computer stores to keep track of important events. Kernel, services, and application events are all recorded in log files.

In Linux, log files can be categorized as:
+ Application logs
+ Event logs
+ Sevice logs
+ System logs

| Linux Log File | Description |
| --- | --- |
| /var/log/messages | |
| /var/log/auth.log | |
| /var/log/secure | |
| /var/log/boot.log | |
| /var/log/dmesg | |
| /var/log/kern.log | |
| /var/log/cron | |
| /var/log/mysqld.log *or* /var/log/mysql.log | |

:computer: LAB - [Locating Log Files](https://github.com/13sauca13/Cyberops-associate/blob/cc25e3e5e08d598dab6e952b4c27fd441b519d17/4.%20Linux%20overview/4.4.4%20Lab_Locating%20log%20files.pdf)

### 4.5 The Linux File System
There are many different kinds of file systems, varying in properties of speed, flexibility, security, size, structure, logic and more. It is up to the administrator to decide which file system type best suits the operating system and the files it will store.

| Linux File System | Description |
| --- | --- |
| ext2 | |
| ext3 | |
| ext4 | |
| NFS | |
| CDFS | |
| Swap File System | |
| HFS+ | |
| APFS | |
| MBR | |

Mounting is the term used for the process of assigning a directory to a partition. After a successful mount operation, the file system contained on the partition is accessible through the specified directory. In this context, the directory is called the mounting point for that file system.

**ANADIR LO QUE FALTA**

:computer: LAB - [Navigating the Linux Filesystem and Permission Settings](https://github.com/13sauca13/Cyberops-associate/blob/8ea1bb80b1d3cebe20a0eda2284e9cf7d281aa1c/4.%20Linux%20overview/4.5.4%20Lab_Navigating%20the%20linux%20filesystem%20and%20permission%20settings.pdf)

> **Rootkit** is a clandestine computer program designed to provide continued privileged access to a computer while actively hiding its presence. It can "hijack" commands changing the way they behave. `chkrootkit` is a shell script that checks system binaries for rootkit modification.

### 4.6 Working with the Linux GUI

### 4.7 Working on a Linux Host

### 4.8 Linux Basics Summary

## 5. Network Protocols

| :desktop_computer: SOHO :arrow_right: | :house: LAN :arrow_right: | :cityscape: MAN :arrow_right: | :world_map: WAN |
| --- | --- | --- | --- |

### 5.1 Network Communications Process

### 5.2 Communications Protocols
Network protocols provide the means for computers to communicate on networks. Network protocols dictate the message encoding, formatting, encapsulation, size, timing, and delivery options. Networking protocols define a common format and set of rules for exchanging messages between devices.
Internet Layer

+ **Application Layer**
  + Name System
    + DNS - Domain Name System. Translates domain names such as cisco.com, into IP addresses.
  + Host Config
    + DHCPv4 - Dynamic Host Configuration Protocol for IPv4. A DHCPv4 server dynamically assigns IPv4 addressing information to DHCPv4 clients at start-up and allows the addresses to be re-used when no longer needed.
    + DHCPv6 - Dynamic Host Configuration Protocol for IPv6. DHCPv6 is similar to DHCPv4. A DHCPv6 server dynamically assigns IPv6 addressing information to DHCPv6 clients at start-up.
    + SLAAC - Stateless Address Autoconfiguration. A method that allows a device to obtain its IPv6 addressing information without using a DHCPv6 server.
  + Email
    + SMTP - Simple Mail Transfer Protocol. Enables clients to send email to a mail server and enables servers to send email to other servers.
    + POP3 - Post Office Protocol version 3. Enables clients to retrieve email from a mail server and download the email to the client's local mail application.
    + IMAP - Internet Message Access Protocol. Enables clients to access email stored on a mail server as well as maintaining email on the server.
  + File Transfer
    + FTP - File Transfer Protocol. Sets the rules that enable a user on one host to access and transfer files to and from another host over a network. FTP is a reliable, connection-oriented, and acknowledged file delivery protocol.
    + SFTP - SSH File Transfer Protocol. As an extension to Secure Shell (SSH) protocol, SFTP can be used to establish a secure file transfer session in which the file transfer is encrypted. SSH is a method for secure remote login that is typically used for accessing the command line of a device.
    + TFTP - Trivial File Transfer Protocol. A simple, connectionless file transfer protocol with best-effort, unacknowledged file delivery. It uses less overhead than FTP.
  + Web and Web Service
    + HTTP - Hypertext Transfer Protocol. A set of rules for exchanging text, graphic images, sound, video, and other multimedia files on the World Wide Web.
    + HTTPS - HTTP Secure. A secure form of HTTP that encrypts the data that is exchanged over the World Wide Web.
    + REST - Representational State Transfer. A web service that uses application programming interfaces (APIs) and HTTP requests to create web applications.

+ **Transport layer**
  + Connection-Oriented
    + TCP - Transmission Control Protocol. Enables reliable communication between processes running on separate hosts and provides reliable, acknowledged transmissions that confirm successful delivery.
Connectionless
    + UDP - User Datagram Protocol. Enables a process running on one host to send packets to a process running on another host. However, UDP does not confirm successful datagram transmission.

+ **Internet Protocol**
  + IPv4 - Internet Protocol version 4. Receives message segments from the transport layer, packages messages into packets, and addresses packets for end-to-end delivery over a network. IPv4 uses a 32-bit address.
  + IPv6 - IP version 6. Similar to IPv4 but uses a 128-bit address.
  + NAT - Network Address Translation. Translates IPv4 addresses from a private network into globally unique public IPv4 addresses.
    + Messaging
      + ICMPv4 - Internet Control Message Protocol for IPv4. Provides feedback from a destination host to a source host about errors in packet delivery.
      + ICMPv6 - ICMP for IPv6. Similar functionality to ICMPv4 but is used for IPv6 packets.
      + ICMPv6 ND - ICMPv6 Neighbor Discovery. Includes four protocol messages that are used for address resolution and duplicate address detection.
    + Routing Protocols
      + OSPF - Open Shortest Path First. Link-state routing protocol that uses a hierarchical design based on areas. OSPF is an open standard interior routing protocol.
      + EIGRP - EIGRP - Enhanced Interior Gateway Routing Protocol. An open standard routing protocol developed by Cisco that uses a composite metric based on bandwidth, delay, load and reliability.
      + BGP - Border Gateway Protocol. An open standard exterior gateway routing protocol used between Internet Service Providers (ISPs). BGP is also commonly used between ISPs and their large private clients to exchange routing information.

+ **Network Access Layer**
  + Address Resolution
    + ARP - Address Resolution Protocol. Provides dynamic address mapping between an IPv4 address and a hardware address.
  + Data Link Protocols
    + Ethernet - Defines the rules for wiring and signaling standards of the network access layer.
    + WLAN - Wireless Local Area Network. Defines the rules for wireless signaling across the 2.4 GHz and 5 GHz radio frequencies.
>Note: You may see other documentation state that ARP operates at the Internet Layer (OSI Layer 3). However, in this course we state that ARP operates at the Network Access layer (OSI Layer 2) because it's primary purpose is the discover the MAC address of the destination. A MAC address is a Layer 2 address.

| | |
| --- | --- |
| Message Formatting and Encapsulation | |
| Message Size | |
| Message Timing | Message timing includes: **Flow Control**, **Response Timeout**, **Access method** |

### 5.3 Data Encapsulation
Segmentation is the process of dividing a stream of data into smaller units for transmissions over the network.
Packets containing segments for the same destination can be sent over different paths.
This leads to segmenting messages having two primary benefits:
+ Increases speed
+ Increases efficiency

The form that a piece of data takes at any layer is called a *protocol data unit* (**PDU**). Also network protocols require that addresses be used for network communication.
| Layer | PDU | Address |
| --- | :---: | --- |
| Application | **Data** | |
| Transport | **Segment** | Protocol Address |
| Network | **Packet** | Network Host Address|
| Data Link | **Frame** | Physical Address |
| Physical | **Bits** | |

:computer: LAB - [Introduction to Wireshark](https://github.com/13sauca13/Cyberops-associate/blob/fe5b88f0206eb9980a25cfd9a8eca68b575ae9f6/5.%20Network%20protocols/5.3.7%20Lab_Introduction%20to%20wireshark.pdf)

## 6. Ethernet and Internet Protocol (IP)

### 6.1 Ethernet
Ethernet operates in the data link layer and the physical layer. It is a family of networking technologies defined in the IEEE 802.2 ([LLC](https://en.wikipedia.org/wiki/Logical_link_control)) and 802.3 ([MAC](https://en.wikipedia.org/wiki/Medium_access_control) and Physical layer) standards. 
The minimum Ethernet frame size is 64 bytes and the maximum is 1518 bytes. This includes all bytes from the destination MAC address field through the frame check sequence (FCS) field. The preamble field is not included when describing the size of the frame.
Any frame less than 64 bytes in length is considered a “collision fragment” or “runt frame” and is automatically discarded by receiving stations. Frames with more than 1500 bytes of data are considered “jumbo” or “baby giant frames”.

An Ethernet MAC address is a 48-bit binary value expressed as 12 hexadecimal digits (4 bits per hexadecimal digit).

### 6.2 IPv4

### 6.3 Ip Addressing Basics
If sending a packet, the AND operation results in that the packet goes to our own network the packet will be sent using layer 2 addresses (MAC Addresses)

### 6.4 Types of IPv4 Addresses
| Class | Range | Private Block |
| --- | --- | --- |
| A | 0.0.0.0/8 to 127.0.0.0/8 | 10.0.0.0/8 |
| B | 128.0.0.0/16 to 191.255.0.0/16 | 172.16.0.0/12 |
| C | 192.0.0.0/24 to 223.255.255.0/24 | 192.18.0.0/16 |
 > There is also a Class D multicast block consisting of 224.0.0.0 to 239.0.0.0 and a Class E experimental address block consisting of 240.0.0.0 – 255.0.0.0.

### 6.5 The Default Gateway

### 6.6 IPv6
IPv6 addresses are 128 bits in length and written as a string of hexadecimal values. Every four bits is represented by a single hexadecimal digit; for a total of 32 hexadecimal values.
+ Rule 1: Omit leading zeros
+ Rule 2: Double colon ( :: *can be used to replace any single or contiguous string of one or more 16-bit hexet of all zeros*)

The prefix length can range from 0 to 128. The recommended IPv6 prefix length for LANs and most other types of networks is /64. t is strongly recommended to use a 64-bit Interface ID for most networks. This is because stateless address autoconfiguration (SLAAC) uses 64 bits for the Interface ID. It also makes subnetting easier to create and manage.

## 7. Connectivity verification

### 7.1 ICMP
ICMP messages common to both ICMPv4 and ICMPv6 include:
+ Host confirmation
+  Destination or Service Unreachable (Codes: 0-Net Unreachable, 1-Host unreachable, 2-Protocol unreachable, 3-Port unreachable)
+  Time exceeded
+  Route redirection
  
ICMPv6 includes four new protocols as part of the Neighbor Discovery Protocol (ND or NDP).
+ Messaging between an IPv6 router and an IPv6 device:
  + Router Solicitation (RS) message
  + Router Advertisement (RA) message
+ Messaging between IPv6 devices:
  + Neighbor Solicitation (NS) message
  + Neighbor Advertisement (NA) message
 
With these messages we have three cases:
+ Router solicitation: RA are sent by routers using SLAAC. When a host is configured to obtain info usin SLAAC, it will send an RS requesting an RA.
+ Address resolution: **COMPLETAR**
+ Duplicate Address Detection (DAD)

### 7.2 Ping and Traceroute Utilities
+ Ping the loopback: This simply tests IP down through the network layer of IP. An error message indicates that TCP/IP is not operational on the host.
+ Ping the Default Gateway: Test the ability of a host to communicate on the local network.
+ Ping a Remote Host: Test the ability of a local host to communicate across an internetwork.
+ Traceroute (test the path): Using traceroute provides round-trip time for each hop along the path and indicates if a hop fails to respond. The round-trip time is the time a packet takes to reach the remote host and for the response from the host to return. An asterisk (*) is used to indicate a lost or unreplied packet.

ICMP is encapsulated directly into IP packets. ICMP uses message codes to differentiate between different types of ICMP messages.
These are some common message codes:
+ 0 – Echo reply (response to a ping)
+ 3 – Destination Unreachable
+ 5 – Redirect (use another route to your destination)
+ 8 – Echo request (for ping)
+ 11 – Time Exceeded (TTL became 0)

The optional ICMP payload field can be used in an attack vector to exfiltrate data.

:memo: 

## 8. Address Resolution Protocol

### 8.1 MAC and IP
IP addresses are used to identify the address of the original source device and the final destination device. The destination IP address may be on the same IP network as the source or may be on a remote network.
Ethernet MAC addresses are used to deliver the data link frame with the encapsulated IP packet from one NIC to another NIC on the same network.
+ If the destination IP address is on the same network, the destination MAC address will be that of the destination device.
+ When the destination IP address is on a remote network, the destination MAC address will be the address of the host’s default gateway.

### 8.2 ARP
ARP is what you need to map IPv4 addresses to MAC addresses, it provides two basic functions:
+ Resolving IPv4 addresses to MAC addresses
+ Maintaining a table of IPv4 to MAC address mappings

:computer: LAB - [Using Wireshark to Examine Ethernet Frames](https://github.com/13sauca13/Cyberops-associate/blob/2db3d276b8ec86645edeac36f8dfef2632eea249/8.%20Address%20resolution%20protocol/8.2.8%20Lab_Using%20wireshark%20to%20examine%20ethernet%20frames.pdf)

### 8.3 ARP Issues


## 9. The Transport Layer

### 9.1 Transport Layer Characteristics
The transport layer includes two protocols:
+ Transmission Control Protocol (TCP)
+ User Datagram Protocol (UDP)

| | TCP | UDP |
| --- | --- | ---|
| Header | 20 Bytes | 8 bytes |
| Data division | Segments | Datagrams |

**CONTINUAR**

### 9.2 Transport Layer Session Establishment
In TCP the client request a service to the server using the port used by the server and dynamically generating a source port number.
The host client establishes the connection with the server using the three-way handshake process:
1. **SYN**: The initiating client requests a client-to-server communication session with the server.
2. **ACK and SYN**: The server acknowledges the client-to-server communication session and requests a server-to-client communication session.
3. **ACK**: The initiating client acknowledges the server-to-client communication session.

>ACK contains the numbre of **THE NEXT EXPECTED PACKET**, not the one received

To close a connection, the Finish (FIN) control flag must be set in the segment header. To end each one-way TCP session, a two-way handshake, consisting of a FIN segment and an Acknowledgment (ACK) segment, is used. Therefore, to terminate a single conversation supported by TCP, four exchanges are needed to end both sessions.
1. **FIN**: When the client has no more data to send in the stream, it sends a segment with the FIN flag set.
2. **ACK**: The server sends an ACK to acknowledge the receipt of the FIN to terminate the session from client to server.
3. **FIN**: The server sends a FIN to the client to terminate the server-to-client session.
4. **ACK**: The client responds with an ACK to acknowledge the FIN from the server.

:computer: LAB - [Using wireshark to observe the tcp 3 way handshake](https://github.com/13sauca13/Cyberops-associate/blob/e65d97d91453578ff76c677090f779826ac4504d/9.%20The%20Transport%20Layer/9.2.6%20Lab_Using%20wireshark%20to%20observe%20the%20tcp%203%20way%20handshake.pdf)

### 9.3 Transport Layer Reliability

**CONTINUAR**

:computer: LAB - [Exploring NMAP](https://github.com/13sauca13/Cyberops-associate/blob/0d3cb8f6b91b76422aba17737c105381ee73372a/9.%20The%20Transport%20Layer/9.3.8%20Lab_Exploring%20nmap.pdf)

## 10. Network Services

### 10.1 DHCP
![DHCP Operation](https://github.com/13sauca13/Cyberops-associate/blob/4e623ca4a8b7ffe5b871e34c6a7a1f6b068ae8c2/Resources/DHCP%20Operation.png)
1. The client broadcasts a DHCP discover (DHCPDISCOVER) message to identify any available DHCP servers on the network. A DHCP server replies with a DHCP offer (DHCPOFFER) message, which offers a lease to the client. The offer message contains the IPv4 address and subnet mask to be assigned, the IPv4 address of the DNS server, and the IPv4 address of the default gateway. The lease offer also includes the duration of the lease.
2. The client may receive multiple DHCPOFFER messages if there is more than one DHCP server on the local network. Therefore, it must choose between them, and sends a DHCP request (DHCPREQUEST) message that identifies the explicit server and lease offer that the client is accepting. A client may also choose to request an address that it had previously been allocated by the server.
3. The server returns a DHCP acknowledgment (DHCPACK) message that acknowledges to the client that the lease has been finalized. If the offer is no longer valid, then the selected server responds with a DHCP negative acknowledgment (DHCPNAK) message. If a DHCPNAK message is returned, then the selection process must begin again with a new DHCPDISCOVER message being transmitted. After the client has the lease, it must be renewed prior to the lease expiration through another DHCPREQUEST message.

**DHCPv4 messages that are sent from the client use UDP source port 68 and destination port 67. DHCPv4 messages sent from the server to the client use UDP source port 67 and destination port 68.**

### 10.2 DNS
The DNS consists of a hierarchy of generic top-level domains (gTLD) which consist of .com, .net, .org, .gov, .edu, and numerous country-level domains, such as .br (Brazil), .es (Spain), .uk (United Kingdom), etc.
At the next level of the DNS hierarchy are second-level domains. These are represented by a domain name that is followed by a top-level domain. Subdomains are found at the next level of the DNS hierarchy and represent some division of the second-level domain. Finally, a fourth level can represent a host in a subdomain.

**COMPLETATR**

