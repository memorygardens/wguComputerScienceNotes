## Terms
#### ping

Ping is one of the most basic tools for testing connectivity to other hosts. It sends an internet control message protocol (ICMP) echo request to a host and listens for the reply. If a reply is received, it will display the time it took and the time to live (TTL) left. Ping has many options for setting attributes of the request, like the maximum TTL, IPv4/IPv6, and the number of requests to send. Ping is useful in troubleshooting connectivity with other devices. If a reply is not received, you will receive a timeout message, which could indicate connectivity issues, firewall issues, or both issues with the other device. In addition, due to the time to get a response, the latency between two devices can be measured, enabling a network engineer to troubleshoot performance problems or a network architect to determine where to place devices to minimize response time to other systems and users.

#### traceroute/tracert

Traceroute and tracert are used to trace the route an IP packet takes to a destination. It displays each hop (next router) in a numerical list with the hop’s IP address and the time it takes to receive the packet. The command traceroute is used for Linux systems and tracert is used for Windows systems. It can be useful in determining where a ping fails, troubleshooting performance issues, and other aspects regarding connectivity.

#### tracepath

Tracepath is similar to traceroute or tracert in that it displays the path taken by a packet from its source to its destination. Tracepath is useful because it can be used by any user instead of needing superuser privileges. It is primarily used in Linux.

#### ipconfig

Ipconfig (internet protocol configuration) provides the user with the IP, subnet mask, and default gateway for each network adapter by default with the /all option information, such as MAC address, DHCP status, and lease information. The command ipconfig/release can be used to release all connections and renew all adapters. It is primarily used in Windows.

#### ifconfig

Similar to ipconfig, ifconfig is used to configure the kernel network interfaces. It is implemented at the time of booting to configure the necessary interfaces. Once the interfaces are configured, it is used for debugging or tuning the system. It is primarily used in Linux.

#### ARP

ARP (Address Resolution Protocol) displays the IP to physical (MAC) address mappings for hosts that have been discovered in the ARP cache. ARP can be used to add, remove, or modify entries in the ARP cache. The hosts need to be on the local network, as these addresses are discovered by broadcasting to everyone on the network and noting the reply from the owner; broadcast traffic is not allowed through a router so that the system will maintain the MAC address of the router.

#### netstat

Netstat (network statistics) displays information about active ports and their state and can be useful in troubleshooting and capacity management. The command netstat -r displays routing information for network adapters. It is available in Windows, MacOS, and Linux.

#### nslookup

Nslookup (name server lookup) displays information for displaying DNS information and troubleshooting DNS problems. It is useful in displaying names to IP address mappings.

#### dig

Dig (domain information groper) is a command used to query the DNS name servers. It is helpful in troubleshooting DNS problems. It is also used for lookups and will display answers from the query. It is a replacement for nslookup.

#### whois

Whois is a tool most often used to look up who owns a domain or block of IP addresses on the internet, including name, email address, and physical address. However, there are many privacy options that hide this information from being returned. It is primarily used in Linux.

#### route

Route can be used to display the current route tables on a host. Route can also be used to add or remove routes. This is used by the local host to determine where to send traffic (0.0.0.0 means the default gateway, where the router sends things if it is not otherwise defined in the routing table).

#### scp

The SCP (Secure Copy Protocol) command is used to securely copy files between servers, leveraging SSH (secure shell) for authentication and encryption.

#### ftp

FTP (file transfer protocol) copies the file from one host to another host. The data is unencrypted. If encryption is needed, FTPS uses SSL/TLS (Secure Sockets Layer, replaced by Transport Layer Security; the same encryption used in https). Transfer uses TCP (transmission control protocol) for reliability and is often used on the internet and other wide-area networks, where errors may be more common.

#### tftp

TFTP (trivial file transfer protocol) transfers a file from either a client to a server or from a server to a client using UDP (user datagram protocol) instead of TCP, and so it is usually used on reliable (local) networks.

#### finger

Finger displays information about a user or users on a remote system, including things such as last log-in time and username. It is primarily used in Linux.

#### nmap

Nmap (Network Mapper) scans networks to see what it can find in terms of hosts and open ports (including well-known ones for many applications). It is commonly used to determine what is deployed on a network for vulnerability analysis, security scans, and related activities. Nmap is not native to either Linux or Windows but can be downloaded for free and used with both.

#### tcpdump

Tcpdump displays TCP/IP packets and other network packets that are being transmitted over the network system. It is a form of protocol analyzer (sometimes called a sniffer) and is designed to show the contents of network packets in human-readable form for troubleshooting, security analysis, etc. Tcpdump is not native to either Linux or Windows but can be downloaded for free and used with both.

#### telnet/ssh

Telnet and SSH (secure shell) allow a user to manage accounts and devices remotely. The main difference between the two is that SSH is encrypted, and thus all data is secure from eavesdropping, while telnet is unencrypted.

## Short hand
1. TRACEPATH • Displays the path taken by a packet from its source to its destination
	• Can be used by any user, regardless of privileges
	• Primarily used in Linux
2. IPCONFIG
	• Provides the user with the IP, subnet mask, and default gateway for each network
	adapter
	• Can be used to release all connections and renew all adapters
	• Primarily used in Windows
3. TRACEROUTE/TRACERT
	• Used to trace the route an IP packet takes to a destination
	• Displays each hop’s IP address and the time it takes to receive the packet
	• Used for Linux and Windows systems
	• Useful in troubleshooting performance and connectivity issues
4. PING
	• One of the most basic tools
	• Tests connectivity to other hosts
	• Sends an ICMP echo request to a host and listens for the reply
	• Useful in troubleshooting connectivity issues
	• Measures latency between two devices
5. NSLOOKUP • Displays some DNS information
	• Troubleshoots DNS problems
	• Useful in displaying names to IP address mappings
	• Native to both Windows and Linux
6. IFCONFIG
	• Used to configure the kernel network interfaces
	• Implemented at the time of botting to configure the necessary interfaces
	• Used for debugging or tuning the system
	• Primarily used in Linux
7. NETSTAT • Displays information about active ports 
