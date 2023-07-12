# Cyberops-associate

> :movie_camera: [Zero Days](https://archive.org/details/zero.-days.-2016.720p)
>
> :movie_camera: [A long day (with no cybersecurity)](https://www.youtube.com/watch?v=PYXdTIwdkj0)
>
> :movie_camera: [Cyber Security | Short Film](https://www.youtube.com/watch?v=GX_XsdNv1PY)
>
> :movie_camera: [Security Awareness Series](https://staysafeonline.org/resources/security-awareness-episodes/)


## 1. The Danger

### 1.1 War stories
:computer: LAB - [Installing the Virtual Machines](https://github.com/13sauca13/Cyberops-associate/blob/d12192f28574fa7a56a9b230b7290bb7acc8e2ad/Resources/Labs/1.1.5%20Lab_Installing%20the%20virtual%20machines.pdf)

:memo: LAB - [Cybersecurity Case Studies](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/1.1.6%20Lab_Cybersecurity%20case%20studies.pdf)

### 1.2 Threat Actors
Threat actors are individuals or groups of individuals who perform cyberattacks.
+ Amateurs (Script Kiddies)
+ Hacktivist
+ Financial Gain
+ Trade secrets and global politics

:memo: LAB - [Learning the details of attacks](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/1.2.3%20Lab_Learning%20the%20Details%20of%20Attacks.pdf)

### 1.3 Threat impact
Personally identifiable information (PII) is any information that can be used to positively identify an individual.
Two subsets of PII are:
+ PHI (*Personal Health Information*)
+ PSI (*Personal Security Information*)

:memo: LAB - [Visualizing the black hats](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/1.3.4%20Lab_Visualizing%20the%20Black%20Hats.pdf)

:movie_camera: [Zero Days](https://archive.org/details/zero.-days.-2016.720p)

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

:eyes: [Splunk](https://www.splunk.com/), [Alien Vault](https://otx.alienvault.com/), [Security Onion](https://securityonionsolutions.com/)

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

:computer: LAB - [Working with Text Files in the CLI](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/4.2.6%20Lab_Working%20with%20text%20files%20in%20the%20cli.pdf)

:computer: LAB - [Getting Familiar with the Linux Shell](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/4.2.7%20Lab_Getting%20familiar%20with%20the%20linux%20shell.pdf)

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
 
:computer: LAB - [Linux servers](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/4.3.4%20Lab_Linux%20servers.pdf)

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

:computer: LAB - [Locating Log Files](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/4.4.4%20Lab_Locating%20log%20files.pdf)

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

:computer: LAB - [Navigating the Linux Filesystem and Permission Settings](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/4.5.4%20Lab_Navigating%20the%20linux%20filesystem%20and%20permission%20settings.pdf)

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

:computer: LAB - [Introduction to Wireshark](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/5.3.7%20Lab_Introduction%20to%20wireshark.pdf)

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

:memo: LAB - [Verify IPv4 and IPv6 Addressing](https://github.com/13sauca13/Cyberops-associate/blob/8a48a9c6a5f2f361b5fcfadddfb875118d271e73/Resources/Labs/7.2.8%20Packet%20tracer_Verify%20ipv4%20and%20ipv6%20addressing.pdf)

:paperclip: LAB - [.pka file Verify IPv4 and IPv6 Addressing](https://github.com/13sauca13/Cyberops-associate/blob/8a48a9c6a5f2f361b5fcfadddfb875118d271e73/Resources/Labs/7.2.8-packet-tracer---verify-ipv4-and-ipv6-addressing.pka)

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

:computer: LAB - [Using Wireshark to Examine Ethernet Frames](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/8.2.8%20Lab_Using%20wireshark%20to%20examine%20ethernet%20frames.pdf)

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

:computer: LAB - [Using wireshark to observe the tcp 3 way handshake](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/9.2.6%20Lab_Using%20wireshark%20to%20observe%20the%20tcp%203%20way%20handshake.pdf)

### 9.3 Transport Layer Reliability

**CONTINUAR**

:computer: LAB - [Exploring NMAP](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/9.3.8%20Lab_Exploring%20nmap.pdf)

## 10. Network Services

### 10.1 DHCP
![DHCP Operation](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Pictures/DHCP%20Operation.png)
1. The client broadcasts a DHCP discover (DHCPDISCOVER) message to identify any available DHCP servers on the network. A DHCP server replies with a DHCP offer (DHCPOFFER) message, which offers a lease to the client. The offer message contains the IPv4 address and subnet mask to be assigned, the IPv4 address of the DNS server, and the IPv4 address of the default gateway. The lease offer also includes the duration of the lease.
2. The client may receive multiple DHCPOFFER messages if there is more than one DHCP server on the local network. Therefore, it must choose between them, and sends a DHCP request (DHCPREQUEST) message that identifies the explicit server and lease offer that the client is accepting. A client may also choose to request an address that it had previously been allocated by the server.
3. The server returns a DHCP acknowledgment (DHCPACK) message that acknowledges to the client that the lease has been finalized. If the offer is no longer valid, then the selected server responds with a DHCP negative acknowledgment (DHCPNAK) message. If a DHCPNAK message is returned, then the selection process must begin again with a new DHCPDISCOVER message being transmitted. After the client has the lease, it must be renewed prior to the lease expiration through another DHCPREQUEST message.

**DHCPv4 messages that are sent from the client use UDP source port 68 and destination port 67. DHCPv4 messages sent from the server to the client use UDP source port 67 and destination port 68.**

### 10.2 DNS
The DNS consists of a hierarchy of generic top-level domains (gTLD) which consist of .com, .net, .org, .gov, .edu, and numerous country-level domains, such as .br (Brazil), .es (Spain), .uk (United Kingdom), etc.
At the next level of the DNS hierarchy are second-level domains. These are represented by a domain name that is followed by a top-level domain. Subdomains are found at the next level of the DNS hierarchy and represent some division of the second-level domain. Finally, a fourth level can represent a host in a subdomain.

**COMPLETATR**
`ipconfig /displaydns` is used to display all the DNS records in cache

:computer: LAB - [Using wireshark to examine a udp dns capture](https://github.com/13sauca13/Cyberops-associate/blob/6c1260c50021dc0e1110f6ee6dccdf5d4af90fe7/Resources/Labs/10.2.7%20Lab_Using%20wireshark%20to%20examine%20a%20udp%20dns%20capture.pdf)

### 10.3 NAT
**COMPLETAR**

:eyes:[Use Local and Global NAT Terms](https://www.cisco.com/c/en/us/support/docs/ip/network-address-translation-nat/4606-8.html)

### 10.4 File Transfer ans Sharing Services
+ **FTP**: Requires two connections, one for commands and replies (21), the other for the actual file transfer (20)
+ **TFTP**:  Is a simplified file transfer protocol that uses well-known UDP port number 69
+ **SMB**: erver Message Block (SMB) is a client/server file sharing protocol that describes the structure of shared network resources. It is a request-response protocol.

:computer: LAB - [Using Wireshark to examine TCP and UDP captures](https://github.com/13sauca13/Cyberops-associate/blob/1629353f2bedad5b170fb26659703c69bdc503cf/Resources/Labs/10.4.3%20Lab_sing%20wireshark%20to%20examine%20tcp%20and%20udp%20captures.pdf)

### 10.5 EMAIL
Email supports three separate protocols for operation: Simple Mail Transfer Protocol (SMTP), Post Office Protocol (POP), and IMAP. The application layer process that sends mail uses SMTP. A client retrieves email using one of the two application layer protocols: POP or IMAP.
+ **SMTP**: SMTP message formats require a message header and a message body. While the message body can contain any amount of text, the message header must have a properly formatted recipient email address and a sender address.

**COMPLETAR**

### 10.6 HTTP
**COMPLETAR**

:computer: LAB - [Using Wireshark to examine HTTP and HTTPS traffic](https://github.com/13sauca13/Cyberops-associate/blob/1c6820d8cb423e167fff8b30b60154a217a02378/Resources/Labs/10.6.7%20Lab_sing%20wireshark%20to%20examine%20http%20and%20https%20traffic.pdf)

## 11. Network Communication Devices

### 11.1 Network devices
**COMPLETAR**

### 11.2 Wireless Communications
**COMPLETAR**

## 12. Network Security Infrastructure

### 12.1 Network Topologies
Topology diagrams:
+ Physical Topology Diagrams
+ Logical Topology Diagrams

LAN networks are designed using a "Three-Layer Model" including Access Layer, Distribution Layer and Core Layer.
The access layer provides endpoints and users direct access to the network. The distribution layer aggregates access layers and provides connectivity to services. Finally, the core layer provides connectivity between distribution layers for large LAN environments.
Some smaller enterprise networks may implement a two-tier hierarchical design. In a two-tier hierarchical design, the core and distribution layers are collapsed into one layer.

Common security architectures:
+ **Private and public**: Traffic from the private network is permitted and inspected. Only traffic returning from the public network asociated with thaffic originated from the private network is permitted.
+ **Demilitarized Zones (DMZ)**: Is firewall design where there is typically one inside interface connected to the private network, one outside interface connected to the public network, and one DMZ interface.
  + Traffic originating from the private network is inspected as it travels toward the public or DMZ network. This traffic is permitted with little or no restriction. Inspected traffic returning from the DMZ or public network to the private network is permitted.
  + Traffic originating from the DMZ network and traveling to the private network is usually blocked.
  + Traffic originating from the DMZ network and traveling to the public network is selectively permitted based on service requirements.
  + Traffic originating from the public network and traveling toward the DMZ is selectively permitted and inspected. This type of traffic is typically email, DNS, HTTP, or HTTPS traffic. Return traffic from the DMZ to the public network is dynamically permitted.
  + Traffic originating from the public network and traveling to the private network is blocked.
+ **Zone-Based (ZPF)**: A zone is a group of one or more interfaces that have similar functions or features. By default, the traffic between interfaces in the same zone is not subject to any policy and passes freely. However, all zone-to-zone traffic is blocked. In order to permit traffic between zones, a policy allowing or inspecting traffic must be configured.

:memo: LAB - [Identify Packet Flow](https://github.com/13sauca13/Cyberops-associate/blob/483c46b2ecbda2d647af0eef82131766f56503ac/Resources/Labs/12.1.9%20Packet%20tracer_Identify%20packet%20flow.pdf)

:paperclip: LAB - [Identify Packet Flow](https://github.com/13sauca13/Cyberops-associate/blob/483c46b2ecbda2d647af0eef82131766f56503ac/Resources/Labs/12.1.9-packet-tracer---identify-packet-flow.pka)

:eyes: [MAC Address Table Flooding](https://en.wikipedia.org/wiki/MAC_flooding)

### 12.2 Security Devices
#### Firewalls
A firewall is a system, or group of systems, that enforces an access control policy between networks.
All firewalls share some common properties:
+ Firewalls are resistant to network attacks.
+ Firewalls are the only transit point between internal corporate networks and external networks because all traffic flows through the firewall.
+ Firewalls enforce the access control policy.

Firewall Types:
+ **Packet filtering (Stateless)**: They are usually part of a router firewall, which permits or denies traffic based on Layer 3 and Layer 4 information.
+ **Stateful**: They are the most versatile and the most common firewall technologies in use. Stateful firewalls provide stateful packet filtering by using connection information maintained in a state table. Stateful filtering is a firewall architecture that is classified at the network layer. It also analyzes traffic at OSI Layer 4 and Layer 5.
+ **Application Gateway (Proxy firewall)**: Filters information at Layers 3, 4, 5, and 7 of the OSI reference model. Most of the firewall control and filtering is done in software.
+ **Next Generation Firewall (NGFW)**: Go beyond by prividing
  + Integrated intrusion prevention
  + Application awareness and control to see and block risky apps
  + Upgrade paths to include future information feeds
  + Techniques to address evolving security threats

**COMPLETAR**

#### Intrusion Prevention and Detection Devices

**COPLETAR**

### 12.3 Security Services
#### ACLs

:memo: LAB - [ACL Demonstration](https://github.com/13sauca13/Cyberops-associate/blob/92644f984a1f51f0ba6fc433b09fd50097c3d9ae/Resources/Labs/12.3.4%20Packet%20tracer_Acl%20demonstration.pdf)

:paperclip: LAB - [ACL Demonstration](https://github.com/13sauca13/Cyberops-associate/blob/92644f984a1f51f0ba6fc433b09fd50097c3d9ae/Resources/Labs/12.3.4-packet-tracer---acl-demonstration.pka)

#### SNMP
#### Net Flow
#### Port Mirroring
#### Syslog Servers
#### NTP
#### AAA Servers
#### VPN

## 13. Attackers and their tools

### 13.1 Who is attacking our networks?
**COMPLETAR**

### 13.2 Threat actor tools
Common network penetration tools:

| Categories of tols | Description |
| --- | --- |
| Password crackers | |Used to crack or remove passwords (eg: John the ripper, Ophcrack) |
| Wireless hacking tools | Used to hack into a wireless network to detect security vulnerabilities (eg: Aircrack-ng, Kismet) |
| Network scanning and hacking tools | Used to probe network devices for open TCP ar UDP ports (eg: Nmap, SuperScan, masscan) |
| Packet crafting tools | Used to probe and test firewalls robustness (eg: Hping, Scapy) |
| Packet sniffers | Used to capture and analyza network packets (eg: Wireshark, Tcpdump) |
| Rootkit detectors | |
| Fuzzers to search vulnerabilities | |
| Forensics tools | To sniff out any trace of evidence in a particular computer system (eg: Sleuth Kit, Helix) |
| Debuggers | Reverse engineer binary files whe writing exploits an to analyze malware (eg: GDB, WinDbg) |
| Hacking operating systemas | Specially designed operating systems preloaded with tools for hacking (eg: Kali Linux, SELinux) |
| encryption tools | They use algorithm schemes to encode the data (VeraCrypt, CipherShed) |
| vulnerability exploitation tools | Identify whether a remote host is vulnerable to a security attack. (eg: Metasploit, Core Impact) |
| vulnerability scanners | Scan a network or system to identify open ports. They can also be used to scan for known vulnerabilities (eg: Nipper, Securia PSI) |

#### Categories of attacks
| Category of attack | Description |
| --- | --- |
| eavesdropping attack | |
| data modification attack | |
| IP address spoofing attack | |
| password-based attacks | |
| denial-of-service (DoS) attack | |
| man-in-the-middle attack (MiTM) | |
| compromised key attack | |
| sniffer attack | |

## 14. Common threats and attacks

### 14.1 Malware
+ **Viruses**: A type of malware that spreads by inserting a copy of itself into another program.
+ **Trojan Horses**: Software that appears to be legitimate, but it contains malicious code which exploits the privileges of the user that runs it. They can be classified:
  + Remote-access
  + Data-sending
  + Destructive
  + Proxy
  + FTP
  + Security software disabler
  + Denial of Service (DoS)
  + Keylogger
+ **Worms**: Similar to viruses because they replicate and can cause the same type of damage. Specifically, worms replicate themselves by independently exploiting vulnerabilities in networks. Whereas a virus requires a host program to run, worms can run by themselves. Other than the initial infection, they no longer require user participation. Most worm attacks consist of three components:
  + Enabling vulnerability
  + Propagation mechanism
  + Payload
+ **Ransomware**: Malware that denies access to the infected computer system or its data. The cybercriminals then demand payment to release the computer system.
+ **Spyware**: Used to gather information about a user and send the information to another entity without the user’s consent. Spyware can be a system monitor, Trojan horse, Adware, tracking cookies, and key loggers.
+ **Adware**: Displays annoying pop-ups to generate revenue for its author. The malware may analyze user interests by tracking the websites visited.
+ **Scareware**: Scam software which uses social engineering to shock or induce anxiety by creating the perception of a threat.
+ **Phishing**: Attempts to convince people to divulge sensitive information.
+ **Rootkits**: Installed on a compromised system.

:memo: LAB - [Anatomy of malware](https://github.com/13sauca13/Cyberops-associate/blob/07106ea668be59246fcf7ce18189a0d83f1a6b3c/Resources/Labs/14.1.11%20Lab_Anatomy%20of%20malware.pdf)

### 14.2 Common network attacks - Reconnaissance, Access and Social Engineering
+ **Reconnaissance Attacks**: Threat actors use reconnaissance (or recon) attacks to do unauthorized discovery and mapping of systems, services, or vulnerabilities. Recon attacks precede access attacks or DoS attacks.
+ **Access Attacks**: Access attacks exploit known vulnerabilities in authentication services, FTP services, and web services. The purpose of this type of attack is to gain entry to web accounts, confidential databases, and other sensitive information. Threat actors use access attacks on network devices and computers to retrieve data, gain access, or to escalate access privileges to administrator status.
  + Password attacks
  + Spofing attacks
  + Trust exploitations
  + Port redirections
  + Man-in-the-middle
  + Buffer overflow
+ **Social engineering attacks**: Social engineering is an access attack that attempts to manipulate individuals into performing actions or divulging confidential information. [The Social Engineering Toolkit (SET)](https://github.com/trustedsec/social-engineer-toolkit) was designed to help white hat hackers and other network security professionals create social engineering attacks to test their own networks. It is a set of menu-based tools that help launch social engineering attacks.

:memo: LAB - [Social Engineering](https://github.com/13sauca13/Cyberops-associate/blob/a428ecd004c5995fb19a6b3bdfa63658b435e856/Resources/Labs/14.2.8%20Lab_Social%20engineering.pdf)

### 14.3 Network attacks - Denial of Service, Buffer Overflows and Evasion
:eyes: [Live botnet threats worlwide](https://www.spamhaus.com/threat-map/)
+ **DoS and DDos**: Creates some sort of interruption of network services to users, devices, or applications. There are two major types of DoS attacks:
  + Overwhelming Quantity of Traffic
  + Maliciously Formatted Packets
+ **Buffer overflow**: Exploiting the buffer memory by overwhelming it with unexpected values usually renders the system inoperable, creating a DoS attack.
> It is estimated that one third of malicious attacks are the result of buffer overflows.

**Evasion methods**
| Evasion method | Description |
| --- | --- |
| Encryption and tunneling | |
| Resource exhaustion | |
| Traffic fragmentation | |
| Protocol-level misinterpretation | |
| Traffic substitution | |
| Traffic insertion | |
| Pivoting | |
| Rootkits | |
| Proxies | |

## 15. Network monitoring tools

:computer: LAB - [What's going on](https://github.com/13sauca13/Cyberops-associate/blob/42e81f67617ab88d2c2d9d231c580fa1352042fb/Resources/Labs/15.0.3%20Class%20activity_What-s%20going%20on.pdf)

### 15.1 Introduction to Network Monitoring
To determine normal network behavior, network monitoring must be implemented. Various tools are used to help discover normal network behavior including IDS, packet analyzers, SNMP, NetFlow, and others.
Some of these tools require captured network data. There are two common methods used to capture traffic and send it to network monitoring devices:
+ **Network taps, sometimes known as test access points (TAPs)**: A network tap is typically a passive splitting device implemented inline between a device of interest and the network. A tap forwards all traffic, including physical layer errors, to an analysis device while also allowing the traffic to reach its intended destination.
+ **Traffic mirroring using Switch Port Analyzer (SPAN) or other port mirroring.**: Port mirroring enables the switch to copy frames that are received on one or more ports to a Switch Port Analyzer (SPAN) port that is connected to an analysis device.

### 15.2 Introduction to Network Mnitoring Tools
#### Network Protocol Analyzers
#### NetFlow
#### SIEM and SOAR

:memo: LAB -[Logging Network Activity](https://github.com/13sauca13/Cyberops-associate/blob/78e7f639f6413919f1a8a75ebb511784621bd27d/Resources/Labs/15.2.7%20Packet%20tracer_Logging-network-activity.pdf)

:paperclip: LAB - [Logging Network Activity](https://github.com/13sauca13/Cyberops-associate/blob/78e7f639f6413919f1a8a75ebb511784621bd27d/Resources/Labs/15.2.7-packet-tracer---logging-network-activity.pka)

## 16. Attacking the Foundation

### 16.1 IP PDU Details
IP was designed as a Layer 3 connectionless protocol. It provides the necessary functions to deliver a packet from a source host to a destination host over an interconnected system of networks. The protocol was not designed to track and manage the flow of packets. These functions, if required, are performed primarily by TCP at Layer 4.

#### IPv4
| IPv4 Header Field | Description |
| --- | --- |
| Version | Contains a 4-bit binary value set to 0100 that identifies this as an IPv4 packet. |
| Internet Header length | A 4-bit field containing the length of the IP header. The minimum length of an IP header is 20 bytes. |
| Differentiated Services or DiffServ (DS) | 8-bit field used to determine the priority of each packet. The six most significant bits of the DiffServ field are the Differentiated Services Code Point (DSCP). The last two bits are the Explicit Congestion Notification (ECN) bits. |
| Total length | Specifies the length of the IP packet including the IP header and the user data. |
| Identification, Flag, and Fragment offset | These fields are used to fragment and reassemble packets. |
| Time-to-Live (TTL) | 8-bit binary value that is used to limit the lifetime of a packet. |
| Protocol | Field is used to identify the next level protocol. |
| Header checksum | Used to determine if any errors have been introduced during transmission. |
| Source IPv4 Address | The source IPv4 address is always a unicast address. |
| Destination IPv4 Address | the destination IPv4 address of the packet. |
| Options and Padding | This is a field that varies in length from 0 to a multiple of 32 bits. |

![IPv4 Packet Header](https://github.com/13sauca13/Cyberops-associate/blob/c3f4152d7471cb3cfe15b3ff1c4d2beed37f1785/Resources/Pictures/IPv4%20Packet%20Header.png)

#### IPv6
| IPv6 Header Field | Description |
| --- | --- |
| Version | This field contains a 4-bit binary value set to 0110 that identifies this as an IPv6 packet. |
| Traffic Class | This 8-bit field is equivalent to the IPv4 Differentiated Services (DS) field. |
| Flow Label | This 20-bit field suggests that all packets with the same flow label receive the same type of handling by routers. |
| Payload Length | This 16-bit field indicates the length of the data portion or payload of the IPv6 packet. |
| Next Header | This 8-bit field is equivalent to the IPv4 Protocol field. |
| Hop Limit | This 8-bit field replaces the IPv4 TTL field. |
| Source IPv6 Address | 128-bit field identifies the IPv6 address of the sending host. |
| Destination IPv6 Address | 128-bit field identifies the IPv6 address of the receiving host. |

>An IPv6 packet may also contain extension headers (EH) that provide optional network layer information. Extension headers are optional and are placed between the IPv6 header and the payload. EHs are used for fragmentation, security, to support mobility, and more. Unlike IPv4, routers do not fragment routed IPv6 packets.

![IPv6 Packet Header](https://github.com/13sauca13/Cyberops-associate/blob/25ef967bb806725a6aa8e78cd4c65efafcc46626/Resources/Pictures/IPv6%20Packet%20Header.png)

### 16.2 IP Vulnerabilities
+ **ICMP Attacks**: Threat actors use Internet Control Message Protocol (ICMP) echo packets (pings) to discover subnets and hosts on a protected network, to generate DoS flood attacks, and to alter host routing tables.
  + ICMP Flood
+ **Denial-of-Service (DoS)**: Threat actors attempt to prevent legitimate users from accessing information or services.
  + Amplification and Reflection Attacks (:eyes: [smurf6](https://kalilinuxtutorials.com/smurf6/))
+ **Address spoofing attacks**: Similar to a DoS attack, but features a simultaneous, coordinated attack from multiple source machines.
  + Non-blinding spoofing: The threat actor can see the traffic.
  + Blind spoofing: The threat actor cannot see the traffic
+ **Man-in-the-middle attack (MiTM)**: Threat actors position themselves between a source and destination to transparently monitor, capture, and control the communication.
+ **Session hijacking**: Threat actors gain access to the physical network, and then use an MiTM attack to hijack a session.

### 16.3 TCP and UDP Vulnerabilities

:eyes: [QUIC Protocol](https://en.wikipedia.org/wiki/QUIC)
 
#### TCP
TCP segment information appears immediately after the IP header. There are 6 control bits for the TCP segment:
| | |
| --- | --- |
| URG | Urgent pointer |
| ACK | Acknowledgment |
| PSH | Push function |
| RST | Reset the connection |
| SYN | Synchronize sequence numbers |
| FIN | No more data from sender |

TCP Attacks:
+ **TCP Syn Flood**: The TCP SYN Flood attack exploits the TCP three-way handshake. A threat actor continually sending TCP SYN session request packets with a randomly spoofed source IP address to a target. The target device replies with a TCP SYN-ACK packet to the spoofed IP address and waits for a TCP ACK packet. Those responses never arrive. Eventually the target host is overwhelmed with half-open TCP connections, and TCP services are denied to legitimate users.
+ **TCP Reset**: Used to terminate TCP communications between two hosts. TCP uses a four-way exchange to close the TCP connection using a pair of FIN and ACK segments from each TCP endpoint. A TCP connection terminates when it receives an RST bit. This is an abrupt way to tear down the TCP connection and inform the receiving host to immediately stop using the TCP connection. A threat actor could do a TCP reset attack and send a spoofed packet containing a TCP RST to one or both endpoints.
+ **TCP Session Hijacking**: The threat actor must spoof the IP address of one host, predict the next sequence number, and send an ACK to the other host. If successful, the threat actor could send, but not receive, data from the target device.

#### UDP
**COMPLETAR**

## 17. Attacking waht we can do

### 17.1 IP Services

#### ARP
Any client can send an unsolicited ARP Reply called a “gratuitous ARP.” This is often done when a device first boots up to inform all other devices on the local network of the new device’s MAC address. When a host sends a gratuitous ARP, other hosts on the subnet store the MAC address and IP address contained in the gratuitous ARP in their ARP tables.

However, this feature of ARP also means that any host can claim to be the owner of any IP/MAC they choose.

+ **ARP Cache Poisoning**: ARP cache poisoning can be used to launch various man-in-the-middle attacks. (:eyes: [ARPSpoof](https://www.kali.org/tools/dsniff/#arpspoof)
  1. ARP Request
  2. ARP Reply
  3. Spoofed Gratuitous ARP Replies

#### DNS
+ **DNS Open Resolver**: A DNS open resolver answers queries from clients outside of its administrative domain.
+ **DNS Stealth**:
  + Fast Flux: Threat actors use this technique to hide their phishing and malware delivery sites behind a quickly-changing network of compromised DNS hosts. The DNS IP addresses are continuously changed within minutes.
  + Double IP Flux: Threat actors use this technique to rapidly change the hostname to IP address mappings and to also change the authoritative name server. This increases the difficulty of identifying the source of the attack.
  + Domain Generation Algorithms: Threat actors use this technique in malware to randomly generate domain names that can then be used as rendezvous points to their command and control (C&C) servers. (:eyes: [SolarWinds Case](https://www.google.com/search?q=solarwinds+case&client=ubuntu-chr&hs=4t6&ei=M96nZOniAsejkdUP2_ug6Ak&ved=0ahUKEwipyPmxp_z_AhXHUaQEHds9CJ0Q4dUDCA8&uact=5&oq=solarwinds+case&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAzIFCAAQgAQyBQgAEIAEMgYIABAWEB4yBggAEBYQHjIGCAAQFhAeMgYIABAWEB4yBggAEBYQHjIGCAAQFhAeMgYIABAWEB4yBggAEBYQHjoKCAAQRxDWBBCwAzoKCAAQigUQsAMQQzoNCAAQ5AIQ1gQQsAMYAToVCC4QigUQxwEQ0QMQyAMQsAMQQxgCOhcILhCKBRDHARDRAxDIAxCwAxAKEEMYAjoPCC4QigUQyAMQsAMQQxgCOggIABCKBRCRAjoLCC4QrwEQxwEQgARKBAhBGABQ5glYmBBg3xdoAXABeACAAYYBiAGUBJIBAzIuM5gBAKABAcABAcgBE9oBBggBEAEYCdoBBggCEAEYCA&sclient=gws-wiz-serp))
+ **DNS Domain Shadowing**: Domain shadowing involves the threat actor gathering domain account credentials in order to silently create multiple sub-domains to be used during the attacks. These subdomains typically point to malicious servers without alerting the actual owner of the parent domain.
+ **DNS Tunneling**: Threat actors who use DNS tunneling place non-DNS traffic within DNS traffic. This method often circumvents security solutions. For the threat actor to use DNS tunneling, the different types of DNS records such as TXT, MX, SRV, NULL, A, or CNAME are altered.

#### DHCP
A DHCP spoofing attack occurs when a rogue DHCP server is connected to the network and provides false IP configuration parameters to legitimate clients. A rogue server can provide a variety of misleading information:
+ Wrong Default Gateway
+ Wrong DNS Server
+ Wrong IP Address

:computer: LAB [Exploring DNS Traffic](https://github.com/13sauca13/Cyberops-associate/blob/f7a7a1e60cd5c9cabd3f649dce8bb81bee774854/Resources/Labs/17.1.7%20Lab_Exploring%20dns%20traffic.pdf)

### 17.2 Enterprise Services

#### HTTP and HTTPS
Common HTTP Exploits:
+ **Malicious iFrames**: Threat actors compromise a webserver and modify web pages by adding HTML for the malicious iFrame. The HTML links to the threat actor’s webserver. In some instances, the iFrame page that is loaded consists of only a few pixels.
+ **HTTP 302 Cuishoning**: Threat actors use the 302 Found HTTP response status code to direct the user’s web browser to a new location. Threat actors often use legitimate HTTP functions such as HTTP redirects to carry out their attacks.
+ **Domain Shadowing**: The threat actor must first compromise a domain. Then, the threat actor must create multiple subdomains of that domain to be used for the attacks. Hijacked domain registration logins are then used to create the many subdomains needed. After these subdomains have been created, attackers can use them as they wish

#### Email
+ **Attachment-based attacks**
+ **Email spoofing**
+ **Spam emailing**
+ **Open mail relay server**
+ **Homoglyphs**

#### Web-Exposed Databases
+ **Code injection**
+ **SQL Injection**

#### Clinet-side Scripting
+ **Cross-Site Scripting**: Cross-Site Scripting (XSS) is where web pages that are executed on the client-side, within their own web browser, are injected with malicious scripts.
  + Sterod (persistent): This is permanently stored on the infected server and is received by all visitors to the infected page.
  + Reflected (non-persistent): This only requires that the malicious script is located in a link and visitors must click the infected link to become infected.

:computer: LAB - [Attacking a MySQL Database](https://github.com/13sauca13/Cyberops-associate/blob/c6f9ea3622460e5a2073113958584eb34a19d9c5/Resources/Labs/17.2.6%20Lab_Attacking%20a%20mysql%20database.pdf)

:computer: LAB - [Reading Server Logs](https://github.com/13sauca13/Cyberops-associate/blob/c6f9ea3622460e5a2073113958584eb34a19d9c5/Resources/Labs/17.2.7%20Lab_Reading%20server%20logs.pdf)

## 18. Understanding Defense

### 18.1 Defense-in-Depth
+ **Assets**: Anything of value to the organization that must be protected.
+ **Vulnerabilities**: A weakness in a system or its design that could be exploited by a threat actor.
+ **Threats**: Any potential danger to an asset.

### 18.2 Security policies, regulations and standards
+ Business Policies: The policies define standards of correct behavior for the business and its employees. In networking, policies define the activities that are allowed on the network.
  + Company policies: The rules of conduct and the responsibilities.
  + Employee policies: Created and maintained by human resources staff to identify employee salary, pay schedule, employee benefits, work schedule, vacations, and more.
  + Security policies: Set of security objectives for a company, define the rules of behavior for users and administrators, and specify system requirements.
    + Identification and authentication policy
    + Password policies
    + Acceptable Use Policy (AUP)
    + Remote access policy
    + Network maintenance policy
    + Incident handling procedures
  + BYOD policies: This enables employees to use their own mobile devices to access company systems, software, networks, or information.
 
## 19. Access Control
 
### 19.1 Access Control Concepts
:eyes: [Pass the hash hack](https://en.wikipedia.org/wiki/Pass_the_hash)

| CIA :arrow_right: | Confidenciality | Integrity | Availability |
| --- | --- | --- | --- |

Zero trust is a comprehensive approach to securing all access across networks, applications, and environments. The principle of a zero trust approach is, “never trust, always verify.” It has three pillars:
+ Zero Trust for the **Workforce**: People who access.
+ Zero Trust for the **Workloads**: Applications that are running.
+ Zero Trust for the **Workplace**: Phiysical security.

An organization must implement proper access controls to protect its network resources, information system resources, and information:
+ Discretionary access control (DAC)
+ Mandatory access control (MAC)
+ Role-based access control (RBAC)
+ Attribute-based access control (ABAC)
+ Rule-based access control (RBAC)
+ Time-based access control (TAC)

### 19.2 AAA Usage and operation
The Authentication, Authorization, and Accounting (AAA) protocol provides the necessary framework to enable scalable access security.

| AAA Component | Description |
| --- | --- |
| **Authentication** | Users and administrators must prove that they are who they say they are. (AAA authentication provides a centralized way to control access to the network.) |
| **Authorization** | Authorization services determine which resources the user can access and which operations the user is allowed to perform. |
| **Accounting** | Accounting records what the user does, keeps track of how network resources are used. |

#### AAA Authentication
Cisco provides two common methods of implementing AAA services.
+ Local AAA Authentication
+ Server-based AAA Authentication

Centralized AAA is more scalable and manageable than local AAA authentication and therefore, it is the preferred AAA implementation.

A centralized AAA system may independently maintain databases for authentication, authorization, and accounting. It can leverage Active Directory or Lightweight Directory Access Protocol (LDAP) for user authentication and group membership, while maintaining its own authorization and accounting databases.
Devices communicate with the centralized AAA server using either the **Remote Authentication Dial-In User Service (RADIUS)** or **Terminal Access Controller Access Control System (TACACS+)** protocols.

#### AAA Accounting Logs
AAA Accounting collects and reports usage data in AAA logs. These logs are useful for security auditing. The collected data might include the start and stop connection times, executed commands, number of packets, and number of bytes. There are several types of accounting information that can be collected (Network, Sonection, EXEC, System, Command, Resource...)

## 20. Treat Intelligence

### 20.1 Information Sources
To effectively protect a network, security professionals must stay informed about threats and vulnerabilities as they evolve. This is through Cisco Cybersecurity Reports, Security Blogs and Podcasts an Network Intelligence Communities like:

| Organization | Description |
| --- | --- |
| [SANS](https://www.sans.org/emea/) | SysAdmin, Audit, Network, Security (SANS) Institute |
| Mitre | The Mitre Corporation maintains a list of common vulnerabilities and exposures (CVE) used by prominent security organizations. |
| FIRST | Forum of Incident Response and Security Teams (FIRST) is a security organization that brings together a variety of computer security incident response teams from government, commercial, and educational organizations to foster cooperation and coordination in information sharing, incident prevention and rapid reaction. |
| SecurityNewsWire | A security news portal that aggregates the latest breaking news pertaining to alerts, exploits, and vulnerabilities. |
| (ISC)<sup>2</sup> | International Information Systems Security Certification Consortium (ISC2) provides vendor neutral education products and career services |
| CIS | The Center for Internet Security (CIS) is a focal point for cyber threat prevention, protection, response, and recovery for state, local, tribal, and territorial (SLTT) governments through the Multi-State Information Sharing and Analysis Center (MS-ISAC). |

### 20.2 Threat Intelligence Services
Threat intelligence services allow the exchange of threat information such as vulnerabilities, indicators of compromise (IOC), and mitigation techniques.
+ [Cisco Talos](https://www.talosintelligence.com/)
+ Fire Eye (Now called [Trellix](https://www.trellix.com/en-us/index.html))
+ Automated Indicator Sharing (AIS)
+ [Common Vulnerabilities and Exposures (CVE) Database](https://cve.org/)

#### Threat Intelligence Communication Standards
Three common threat intelligence sharing standards include the following:
+ **Structured Threat Information Expression (STIX)**: This is a set of specifications for exchanging cyber threat information between organizations. The Cyber Observable Expression (CybOX) standard has been incorporated into STIX.
+ **Trusted Automated Exchange of Indicator Information (TAXII)**: This is the specification for an application layer protocol that allows the communication of CTI over HTTPS. TAXII is designed to support STIX.
+ **CybOX**: This is a set of standardized schema for specifying, capturing, characterizing, and communicating events and properties of network operations that supports many cybersecurity functions.

## 21. Cryptography

:computer: LAB - [Creating Codes](https://github.com/13sauca13/Cyberops-associate/blob/f057f9544fa87decf69d682902891dd8e7e2fecd/Resources/Labs/21.0.3%20Class%20activity_Creating%20codes.pdf)

### 21.1 Integrity and Authenticity
There are four elements of secure communications:
+ **Data Integrity**
+ **Origin Authentication**
+ **Data Confidentiality**
+ **Data Non-Repudiation**

Hashes are used to verify and ensure data integrity. Hashing is based on a one-way mathematical function that is relatively easy to compute, but significantly harder to reverse. There are four well-known hash functions:
+ MD5 with 128-bit digest
+ SHA-1
+ SHA-2: It includes SHA-224 (224 bit), SHA-256 (256 bit), SHA-384 (384 bit), and SHA-512 (512 bit).
+ SHA-3: SHA-3 is the newest hashing algorithm. Includes SHA3-224 (224 bit), SHA3-256 (256 bit), SHA3-384 (384 bit), and SHA3-512 (512 bit).

To add origin authentication and integrity assurance, use a keyed-hash message authentication code (HMAC). HMAC uses an additional secret key as input to the hash function.

:computer: LAB - [Hashing Things Out](https://github.com/13sauca13/Cyberops-associate/blob/3597348d9af9042e00a0046ee8e70d6d86ed5854/Resources/Labs/21.1.6%20Lab_Hashing%20things%20out.pdf)

### 21.2 Confidentiality
There are two classes of encryption used to provide data confidentiality; asymmetric and symmetric.

#### Symetric Encryption
Symmetric algorithms use the same pre-shared key to encrypt and decrypt data. A pre-shared key, also called a secret key, is known by the sender and receiver before any encrypted communications can take place. Data can be ciphered by block or stream.
(eg: Data Encryption Standard (DES), 3DES (Triple DES), Advanced Encryption Standard (AES), Software-Optimized Encryption Algorithm (SEAL), Rivest Ciphers (RC) series algorithms)

#### Asymetric Encryption
Asymmetric algorithms use a public key and a private key. Both keys are capable of the encryption process, but the complementary paired key is required for decryption. The process is also reversible. Data that is encrypted with the public key requires the private key to decrypt.
(eg: Internal Key Exchange (IKE), Secure Socket Layer (SSL), Secure Shell (SSH), Pretty Good Privacy (PGP)

:computer: LAB - [Encrypting and decrypting data using openssl](https://github.com/13sauca13/Cyberops-associate/blob/bd3ef47baf095f3519f0c82ee6d22b5362e25628/Resources/Labs/21.2.10%20Lab_Encrypting%20and%20decrypting%20data%20using%20openssl.pdf)

:computer: LAB - [Encrypting and Decrypting Data using a Hacker Tool](https://github.com/13sauca13/Cyberops-associate/blob/bd3ef47baf095f3519f0c82ee6d22b5362e25628/Resources/Labs/21.2.11%20Lab_Encrypting%20and%20decrypting%20data%20using%20a%20hacker%20tool.pdf)

:computer: LAB - [Examining telnet and ssh in wireshark](https://github.com/13sauca13/Cyberops-associate/blob/bd3ef47baf095f3519f0c82ee6d22b5362e25628/Resources/Labs/21.2.12%20Lab_Examining%20telnet%20and%20ssh%20in%20wireshark.pdf)

### 21.3 Public Key Cryptography
#### Digital Signatures
Digital signatures are a mathematical technique used to provide authenticity, integrity, and nonrepudiation. Digital signatures have specific properties that enable entity authentication and data integrity. In addition, digital signatures provide nonrepudiation of the transaction. In other words, the digital signature serves as legal proof that the data exchange did take place. Digital signatures use asymmetric cryptography. They can be used for:
+ Code Signing: Digital signatures are commonly used to provide assurance of the authenticity and integrity of software code. Executable files are wrapped in a digitally signed envelope, which allows the end user to verify the signature before installing the software.
+ Digital Certificates: Digital signatures are used to verify that an artifact, such as a file or message, is sent from the verified individual.

### 21.4 Authorities and the PKI Trust System
**COMPLETAR**

:computer: LAB - [Certificate Authority Stores](https://github.com/13sauca13/Cyberops-associate/blob/bd69fb9e27d4f0b8b084c1a30d56ad2dccbb5ba6/Resources/Labs/21.4.7%20Lab_Certificate%20authority%20stores.pdf)

### 21.5 Applications and Impacts of Cryptography
+ PKI Applications
+ Encrypted Network Transactions
+ Encryption and Security Monitoring

## 22. Endpoint Protection

### 22.1 Antimalware Protection
:eyes: [AV-TEST](https://www.av-test.org/en/)

Endpoints are hosts on the network that can access or be accessed by other hosts on the network (computers, servers and Internet of Things (IoT) devices)
+ **Host-Based Malware Protection**:
  + Antivirus/Antimalware Software
    + Signature-base: Recognizes various characteristics of known malware files.
    + Heuristics-based: Recognizes general features shared by various types of malware.
    + Behavior-based: Employs analysis of suspicious behavior.
  + Host-based Firewall
  + Host-based Security Suites: Include antivirus, anti-phishing, safe browsing, Host-based intrusion prevention system, and firewall capabilities.
+ **Network-Based Malware Protection**:
  + Advanced Malware Protection (AMP)
  + Email Security Appliance (ESA)
  + Web Security Appliance (WSA)
  + Network Admission Control (NAC)
 
### 22.2 Host-based Intrusion Prevention
#### Host-based Firewalls
Host-based personal firewalls are standalone software programs that control traffic entering or leaving a computer.
+ Windows Defender Firewall
+ iptables
+ nftables
+ TCP Wrappers

#### Host-based Intrusion Detection
A host-based intrusion detection system (HIDS) is designed to protect hosts against known and unknown malware. A HIDS can perform detailed monitoring and reporting on the system configuration and application activity. It can provide log analysis, event correlation, integrity checking, policy enforcement, rootkit detection, and alerting. A HIDS will frequently include a management server endpoint.
Host-based security systems function as both detection and prevention systems.
(eg: Cisco AMP, AlienVault, Tripwire, Open Source HIDS SECurity (OSSEC))

### 22.3 Application Security
An attack surface is the sum of all vulnerabilities in a given system. The SANS Institute describes three components of the attack surface:
+ Network Attack Surface
+ Software Attack Surface
+ Human Attack Surface

One way of decreasing the attack surface is to limit access to potential threats by creating lists of prohibited applications. This is known as **lock listing**
**Allow lists** are created in accordance with a security baseline that has been established by an organization.
:eyes: [Te Spamhaus Project](https://www.spamhaus.org/)

**Sandboxing** is a technique that allows suspicious files to be executed and analyzed in a safe environment. Automated malware analysis sandboxes offer tools that analyze malware behavior.
(eg: Cuckoo Sandbox, VirusTotal, ANY.RUN)

## 23. Endpoint Vulnerability Assessment

### 23.1 Network and Server Profiling
#### Network profiling
It provides a statistical baseline that serves as a reference poin for normal operation. The most important elements of the network profile are:
| Network Profile Element | Description |
| --- | --- |
| Session Duration | This is the time between the establishment of a data flow and its termination. |
| Total throughput | This is the amount of data passing from a given source to a given destination in a given period of time. |
| Ports used | This is a list of TCP or UDP processes that are available to accept data. |
| Critical asset address space | These are the IP addresses or the logical location of essential systems or data. |

Server profiling is used to establish the accepted operating state of servers. A server profile is a security baseline for a given server. It establishes the network, user, and application parameters that are accepted for a specific server

#### Network Anomaly Detection
One approach to detection of network attacks is the analysis of the diverse, unstructured data (such as such as the features of packet flow, features of the packets themselves, and telemetry from multiple sources) using Big Data analytics techniques. This is known as network behavior analysis (NBA).

### 23.2 Comon Vulnerability Scoring System (CVSS)
The Common Vulnerability Scoring System (CVSS) is a risk assessment tool that is designed to convey the common attributes and severity of vulnerabilities in computer hardware and software systems. It is a vendor-neutral, industry standard, open framework for weighting the risks of a vulnerability using a variety of metrics.
:eyes: [Forum of Incident Response and Security Teams (FIRST)]([https://www.first.org/](https://www.first.org/cvss/calculator/3.0)https://www.first.org/cvss/calculator/3.0)

**COMPLETAR**

Other vunerability information sources:
+ Common Vulnerabilities and Exposures (CVE)
+ National Vulnerability Database (NVD)

### 23.3 Secure Device Management
Risk management involves the selection and specification of security controls for an organization, is an ongoing, multi-step, cyclical process:
+ Risk identification
+ Risck assessment
+ Risk response plannin
+ Response implementation
+ Monitor assess results

Risk is determined as the relationship between threat, vulnerability, and the nature of the organization.

#### Movile Device Management
MDM systems, such as Cisco Meraki Systems Manager, allow security personnel to configure, monitor and update a very diverse set of mobile clients from the cloud.

#### Configuration Management
Configuration management addresses the inventory and control of hardware and software configurations of systems. Secure device configurations reduce security risk.
(eg: Puppet, Chef, Ansible, SaltStack)

#### Enterprise Patch Management
Patch management involves all aspects of software patching, including identifying required patches, acquiring, distributing, installing, and verifying that the patch is installed on all required systems. Installing patches is frequently the most effective way to mitigate software vulnerabilities.
(eg: SolarWinds, LANDesk, Microsoft System Center Configuration Manager (SCCM))

### 23.4 Information Security Management Systems
An Information Security Management System (ISMS) consists of a management framework through which an organization identifies, analyzes, and addresses information security risks. ISMSs are not based in servers or security devices. Instead, an ISMS consists of a set of practices that are systematically applied by an organization to ensure continuous improvement in information security. ISMSs provide conceptual models that guide organizations in planning, implementing, governing, and evaluating information security programs.

####ISO-270001
The ISO 27001 certification is a global, industry-wide specification for an ISMS.

#### NIST Cybersecurity Framework
NIST has also developed the Cybersecurity framework which is similar to the ISO/IEC 27000 standards. The NIST framework is a set of standards designed to integrate existing standards, guidelines, and practices to help better manage and reduce cybersecurity risk.

## 24. Technologies and Protocols

### 24.1 Monitoring Common Protocols

#### Syslog and NTP
Servers that run syslog typically listen on UDP port 514.
Syslog and Network Time Protocol (NTP) are essential to the work of the cybersecurity analyst. The syslog standard is used for logging event messages from network devices and endpoints
Syslog messages are usually timestamped. This allows messages from different sources to be organized by time to provide a view of network communication processes. Because the messages can come from many devices, it is important that the devices share a consistent timeclock. One way that this can be achieved is for the devices to use Network Time Protocol (NTP). NTP uses a hierarchy of authoritative time sources to share time information between devices on the network, as shown in the figure. In this way, device messages that share consistent time information can be submitted to the syslog server. NTP operates on UDP port 123.
Threat actors may attempt to attack the NTP infrastructure in order to corrupt time information used to correlate logged network events. This can serve to obfuscate traces of ongoing exploits.

#### DNS
DNS is now used by many types of malware. Some varieties of malware use DNS to communicate with command-and-control (CnC) servers and to exfiltrate data in traffic disguised as normal DNS queries. Various types of encoding, such as Base64, 8-bit binary, and Hex can be used to camouflage the data and evade basic data loss prevention (DLP) measures.

#### HTTP and HTTPS
HTTP does not protect data from alteration or interception by malicious parties, which is a serious threat to privacy, identity, and information security.
Network security services, such as Cisco Web Reputation filtering, can detect when a website attempts to send content from an untrusted website to the host, even when sent from an iFrame.

#### EMAIL
Email protocols such as SMTP, POP3, and IMAP can be used by threat actors to spread malware, exfiltrate data, or provide channels to malware CnC servers.

#### ICMP
ICMP can be used to identify hosts on a network, the structure of a network, and determine the operating systems at use on the network. It can also be used as a vehicle for various types of DoS attacks.
ICMP can also be used for data exfiltration.
:eyes: [Loki Exploit](https://www.skillset.com/questions/the-hacking-tool-loki-provides-shell-access-to-the-attacker-over-6083)

### 24.2 Security Technologies
Many technologies and protocols can have impacts on security monitoring:
+ **ACLs**
+ **NAT and PAT**
+ **Encryption, Encapsulation and Tuneling**
+ **Peer-to-peer networking and Tor**
+ **Load Balancing**

## 25. Network Security Data

### 25.1 Types of Security Data

#### Alert Data
Alert data consists of messages generated by intrusion prevention systems (IPSs) or intrusion detection systems (IDSs) in response to traffic that violates a rule or matches the signature of a known exploit. A network IDS (NIDS), such as Snort, comes configured with rules for known exploits. Alerts are generated by Snort and are made readable and searchable by the Sguil and Squert applications, which are part of the Security Onion suite of NSM tools.

#### Session and Transaction Data
Session data is a record of a conversation between two network endpoints, which are often a client and a server. Session data is data about the session, not the data retrieved and used by the client. Transaction data consists of the messages that are exchanged during network sessions. These transactions can be viewed in packet capture transcripts.
Zeek, formerly Bro, is a network security monitoring tool

![Zeek Session Data](https://github.com/13sauca13/Cyberops-associate/blob/033d3145b6d937325873a185e92bf1ccad2baa0c/Resources/Pictures/Zeek%20Session%20Data.png)

#### Full Packet Captures
Full packet captures are the most detailed network data that is generally collected. Because of the amount of detail, they are also the most storage and retrieval intensive types of data used in NSM. Full packet captures contain not only data about network conversations, like session data. Full packet captures also contain the actual contents of the conversations.

#### Statistical Data
Statistical data is about network traffic. Statistical data is created through the analysis of other forms of network data. Conclusions can be made that describe or predict network behavior from these analysis. Statistical characteristics of normal network behavior can be compared to current network traffic in an effort to detect anomalies.

### 25.2 End Device Logs

#### Host Logs
HIDS not only detects intrusions, but in the form of host-based firewalls, can also prevent intrusion. This software creates logs and stores them on the host.
Microsoft Windows host logs are visible locally through Event Viewer. Event Viewer keeps five types of logs:
+ Application logs
+ System logs
+ Setup logs
+ Security logs
+ Command-line logs
Various logs can have different event types: Error, Warning, Information, Success Audit, Failure Audit.

#### Syslog
Syslog incudes specifications for message formats, a client-server application structure, and network protocol. Syslog was defined within the Syslog working group of the IETF (RFC 5424) and is supported by a wide variety of devices and receivers across multiple platforms.
The full format of a Syslog message that is seen on the network has three distinct parts and a total of 1024 bytes:
| PRI (priority) | HEADER | MSG (message text) |
| --- | --- | --- |
> Priority=(Facility*8)+Severity

#### Server Logs
Server logs are an essential source of data for network security monitoring. Network application servers such as email and web servers keep access and error logs.

#### SIEM and Log Collection
Security Information and Event Management (SIEM) technology is used in many organizations to provide real-time reporting and long-term analysis of security events

### 25.3 Network Logs

#### Tcpdump
The tcpdump command line tool is a very popular packet analyzer. It can display packet captures in real time or write packet captures to a file. It captures detailed packet protocol and content data. Wireshark is a GUI built on tcpdump functionality.

#### NetFlow
NetFlow is a protocol that was developed by Cisco as a tool for network troubleshooting and session-based accounting.
NetFlow does not do a full packet capture or capture the actual content in the packet. NetFlow records information about the packet flow including metadata.

#### Application Visibility and Control
The Cisco Application Visibility and Control (AVC) system that combines multiple technologies to recognize, analyze, and control over 1000 applications. These include voice and video, email, file sharing, gaming, peer-to-peer (P2P), and cloud-based applications.
AVC uses Cisco next-generation network-based application recognition version 2 (NBAR2), also known as Next-Generation NBAR, to discover and classify the applications in use on the network. The NBAR2 application recognition engine supports over 1000 network applications.

#### Content Filter Logs
Devices that provide content filtering, such as the Cisco Email Security Appliance (ESA) and the Cisco Web Security Appliance (WSA), provide a wide range of functionalities for security monitoring. Logging is available for many of these functionalities.

#### Logging from CISCO Devices
Cisco security devices can be configured to submit events and alerts to security management platforms using SNMP or syslog.

![Cisco syslog messages](https://github.com/13sauca13/Cyberops-associate/blob/f9373220ed4556b84678a4e9a3394e563ac90d50/Resources/Pictures/Cisco%20syslog%20message.png)

#### Proxy logs
Proxy servers, such as those used for web and DNS requests, contain valuable logs that are a primary source of data for network security monitoring.
Proxy servers are devices that act as intermediaries for network clients.

#### Next-generation Firewalls
Next-Generation or NextGen Firewall devices extend network security beyond IP addresses and Layer 4 port numbers to the application layer and beyond.
Common NGFW events include:
+ Connection event
+ Intrusion event
+ Host or Endpoint event
+ Network Discovery event
+ Netflow event

:memo: LAB - [Explore NetFlow Implementation](https://github.com/13sauca13/Cyberops-associate/blob/b79a695e06c0331814712dc9b9955a6f5edea2fb/Resources/Labs/25.3.10%20Packet%20tracer_Explore%20a%20netflow%20implementation.pdf)

:paperclip: LAB - [Explore NetFlow Implementtion](https://github.com/13sauca13/Cyberops-associate/blob/b79a695e06c0331814712dc9b9955a6f5edea2fb/Resources/Labs/25.3.10-packet-tracer---explore-a-netflow-implementation.pka)

:memo: LAB - [Logging from multiple sources](https://github.com/13sauca13/Cyberops-associate/blob/b79a695e06c0331814712dc9b9955a6f5edea2fb/Resources/Labs/25.3.11%20Packet%20tracer_Logging%20from%20multiple%20sources.pdf)

:paperclip: LAB - [Logging from multiple sources](https://github.com/13sauca13/Cyberops-associate/blob/b79a695e06c0331814712dc9b9955a6f5edea2fb/Resources/Labs/25.3.11-packet-tracer---logging-from-multiple-sources.pka)

## 26. Evaluating Alerts

### 26.1 Sources of Alerts

#### Security Onion
Security Onion is an open-source suite of Network Security Monitoring (NSM) tools that run on an Ubuntu Linux distribution. Security Onion tools provide three core functions for the cybersecurity analyst: full packet capture and data types, network-based and host-based intrusion detection systems, and alert analyst tools.Security Onion is an open-source suite of Network Security Monitoring (NSM) tools that run on an Ubuntu Linux distribution. Security Onion tools provide three core functions for the cybersecurity analyst: full packet capture and data types, network-based and host-based intrusion detection systems, and alert analyst tools.
![Security Onion Architecture](https://github.com/13sauca13/Cyberops-associate/blob/863963975387a9dbbb4b3308c97380797f95596a/Resources/Pictures/Security%20Onion%20architecture.png)

+ Analysis:
  +  Sguil: A high-level console for investigating security alerts from a wide variety of sources. Sguil serves as a starting point in the investigation of security alerts.
  +  Kibana: Dashboard for Elasticsearch.
  +  Wireshark: GUI based analyzer and packet capture tool.
+ Detection:
  + CapMe: Web application that allows viewing of pcap transcripts rendered with the tcpflow or Zeek tools. CapME can be accessed from the Enterprise Log Search and Archive (ELSA) tool.
  + Snort: This is a Network Intrusion Detection System (NIDS). It is an important source of alert data that is indexed in the Sguil analysis tool. Snort uses rules and signatures to generate alerts.
  + Zeek: Formerly known as Bro. Rather than using signatures or rules, Zeek uses policies, in the form of scripts that determine what data to log and when to issue alert notifications. It can also submit file attachments for malware analysis, block access to malicious locations, and shut down a computer that appears to be violating security policies.
  + OSSEC: This is a host-based intrusion detection system (HIDS), it monitors host system operations, including conducting file integrity monitoring, local log monitoring, system process monitoring, and rootkit detection. OSSEC alerts and log data are available to Sguil and Kibana.
  + Wazuh: HIDS that will replace OSSEC.
  + Suricata: NIDS that uses a signature-based approach.

Security alerts are notification messages that are generated by NSM tools, systems, and security devices, Sguil provides a console that integrates alerts from multiple sources into a timestamped queue.
Alerts can come from a number of sources:
+ NIDS: Snort, Zeek and Suricata
+ HIDS: OSSEC and Wazuh
+ Asset manageent and monitoring: Passive Asset Detection Sytem (PADS)
+ HTTPS, DNS and TCP transactions: Recorded by Zeek and pcaps
+ Syslog messages: Multiple sources

:exclamation: [Check Snort rule structure](https://contenthub.netacad.com/cyberops/26.1.6)

:computer: LAB - [Snort and Firewall Rules](https://github.com/13sauca13/Cyberops-associate/blob/cd016459ffc27a9304fd4f9202d147a02e1042c1/Resources/Labs/26.1.7%20Lab_Snort%20and%20firewall%20rules.pdf)
