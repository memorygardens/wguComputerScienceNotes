### ping

Ping is one of the most basic tools for testing connectivity to other hosts. It sends an internet control message protocol (ICMP) echo request to a host and listens for the reply. If a reply is received, it will display the time it took and the time to live (TTL) left. Ping has many options for setting attributes of the request, like the maximum TTL, IPv4/IPv6, and the number of requests to send. Ping is useful in troubleshooting connectivity with other devices. If a reply is not received, you will receive a timeout message, which could indicate connectivity issues, firewall issues, or both issues with the other device. In addition, due to the time to get a response, the latency between two devices can be measured, enabling a network engineer to troubleshoot performance problems or a network architect to determine where to place devices to minimize response time to other systems and users.

### traceroute/tracert

Traceroute and tracert are used to trace the route an IP packet takes to a destination. It displays each hop (next router) in a numerical list with the hop’s IP address and the time it takes to receive the packet. The command traceroute is used for Linux systems and tracert is used for Windows systems. It can be useful in determining where a ping fails, troubleshooting performance issues, and other aspects regarding connectivity.

### tracepath

Tracepath is similar to traceroute or tracert in that it displays the path taken by a packet from its source to its destination. Tracepath is useful because it can be used by any user instead of needing superuser privileges. It is primarily used in Linux.

### ipconfig

Ipconfig (internet protocol configuration) provides the user with the IP, subnet mask, and default gateway for each network adapter by default with the /all option information, such as MAC address, DHCP status, and lease information. The command ipconfig/release can be used to release all connections and renew all adapters. It is primarily used in Windows.

### ifconfig

Similar to ipconfig, ifconfig is used to configure the kernel network interfaces. It is implemented at the time of booting to configure the necessary interfaces. Once the interfaces are configured, it is used for debugging or tuning the system. It is primarily used in Linux.

### ARP

ARP (Address Resolution Protocol) displays the IP to physical (MAC) address mappings for hosts that have been discovered in the ARP cache. ARP can be used to add, remove, or modify entries in the ARP cache. The hosts need to be on the local network, as these addresses are discovered by broadcasting to everyone on the network and noting the reply from the owner; broadcast traffic is not allowed through a router so that the system will maintain the MAC address of the router.

### netstat

Netstat (network statistics) displays information about active ports and their state and can be useful in troubleshooting and capacity management. The command netstat -r displays routing information for network adapters. It is available in Windows, MacOS, and Linux.

### nslookup

Nslookup (name server lookup) displays information for displaying DNS information and troubleshooting DNS problems. It is useful in displaying names to IP address mappings.

### dig

Dig (domain information groper) is a command used to query the DNS name servers. It is helpful in troubleshooting DNS problems. It is also used for lookups and will display answers from the query. It is a replacement for nslookup.

### whois

Whois is a tool most often used to look up who owns a domain or block of IP addresses on the internet, including name, email address, and physical address. However, there are many privacy options that hide this information from being returned. It is primarily used in Linux.

### route

Route can be used to display the current route tables on a host. Route can also be used to add or remove routes. This is used by the local host to determine where to send traffic (0.0.0.0 means the default gateway, where the router sends things if it is not otherwise defined in the routing table).

### scp

The SCP (Secure Copy Protocol) command is used to securely copy files between servers, leveraging SSH (secure shell) for authentication and encryption.

### ftp

FTP (file transfer protocol) copies the file from one host to another host. The data is unencrypted. If encryption is needed, FTPS uses SSL/TLS (Secure Sockets Layer, replaced by Transport Layer Security; the same encryption used in https). Transfer uses TCP (transmission control protocol) for reliability and is often used on the internet and other wide-area networks, where errors may be more common.

### tftp

TFTP (trivial file transfer protocol) transfers a file from either a client to a server or from a server to a client using UDP (user datagram protocol) instead of TCP, and so it is usually used on reliable (local) networks.

### finger

Finger displays information about a user or users on a remote system, including things such as last log-in time and username. It is primarily used in Linux.

### nmap

Nmap (Network Mapper) scans networks to see what it can find in terms of hosts and open ports (including well-known ones for many applications). It is commonly used to determine what is deployed on a network for vulnerability analysis, security scans, and related activities. Nmap is not native to either Linux or Windows but can be downloaded for free and used with both.

### tcpdump

Tcpdump displays TCP/IP packets and other network packets that are being transmitted over the network system. It is a form of protocol analyzer (sometimes called a sniffer) and is designed to show the contents of network packets in human-readable form for troubleshooting, security analysis, etc. Tcpdump is not native to either Linux or Windows but can be downloaded for free and used with both.

### telnet/ssh

Telnet and SSH (secure shell) allow a user to manage accounts and devices remotely. The main difference between the two is that SSH is encrypted, and thus all data is secure from eavesdropping, while telnet is unencrypted.

### PAN

![Personal area network with a laptop in the middle connected to different devices.](https://assets.wgu.edu/9ceee00ba1d975d46758b5bb34956e1a)

Diagram. A Personal Area Network (PAN)

A personal area network, or PAN, is a network that is centered around a person and their devices. A PAN allows for various devices, such as a person’s desktop computer, laptop, smartphone, tablet, headphones, wireless keyboard and mouse, and speakers to communicate with each other, often over Bluetooth in the case of wireless connections or USB in the case of wired connections. PANs can be used to enable communication between the devices, such as a device sending music to speakers or headphones, or can be used as a jumping-off point for other devices to a network gateway, such as when a mobile phone acts as a Wi-Fi hotspot for other devices.

Apple products are a good example of this. Apple has built their products to integrate together via iCloud. Each device is registered to a single user account. When a user account has multiple devices, notifications, workflow, and data are easily shared across them. For example, when a phone call is being received by an iPhone, it also will alert a MacBook and an iPad that are connected to the PAN. The call is able to be answered by any of the devices.

### LAN

![Local Area Network with a router in the middle connected to many devices.](https://assets.wgu.edu/ced45f0e4f5e188f759169071f8e108f)

Diagram. A Local Area Network (LAN)

A local area network, or LAN, consists of computers connected within a limited area. Some examples of LANs are a home, lab, or office building. Most often, LANs use Ethernet, Wi-Fi, or both to connect the network devices.

LANs were popularized in the 1960s for research labs that needed their computers to be connected and able to transfer data at high speeds (at that time). While similar to LANs today, there was significant growth and development through the following decades to LANs. It was not until the 1980s that LANs supported TCP/IP and the commands and programs were often used with it as well as PCs (as opposed to mainframes or minicomputers), which opened the market for even more expansion into LANs as they are known today.

Many LANs are wireless, where users are connected via Wi-Fi and can move unrestricted throughout the coverage area. This is a popular choice for home users and small businesses, as it is easy and inexpensive to install and allows guests to use the network as well.

### WLAN

A wireless local area network, or WLAN, is a LAN with wireless connectivity. Unlike LANs, which are wired, WLANs use Wi-Fi to communicate with devices. Users and devices can be placed anywhere and move anywhere in the coverage area. This is a popular choice for small businesses, as it is easy and inexpensive to install and allows guests to use the network as well with a hotspot service. Many WLANs also act as a gateway to the internet for users.

Many private homes use WLAN in the form of Wi-Fi, as it allows for multiple users to be connected to the network (and usually the broader internet), but not be tied down to a specific location in the home.

![Various devices are connected wirelessly to a wifi router, which is in turn connected to an internet service provider.](https://assets.wgu.edu/4b1bd064c445636b69a8fee3cdd21890)

Diagram. A Wireless Local Area Network (WLAN)

### SAN

A storage area network, or SAN, is a network that allows access to storage devices specifically instead of the more general networking that can be used for any purpose. SANs allow servers to access devices such as tape libraries and disk arrays while presenting them to the operating system like any other locally attached device.

Typically, a SAN is a network dedicated to storage devices and the servers that need access to them. The key reason for this is to reduce interference from normal LAN traffic during data transfer. SANs may also use other protocols, such as Fibre Channels that do not usually operate on traditional network equipment.

![10 gigabit cables connect the servers to an expandable redundant array of independent disks (RAID).](https://assets.wgu.edu/4ea46342123b2960995c71b15a9ac682)

Diagram. Example of a storage area network (SAN)

### CAN

![Campus area network a group of buildings all connected together.](https://assets.wgu.edu/2c87856ec1c3817f81816c2640d47d96)

Diagram. Campus area network (CAN).

A campus area network, or CAN, provides networking of multiple LANs across a limited area, like a university campus or a group of buildings owned by a company. Each LAN would typically be constrained to a single building (or even just a part of a building), and the CAN would link them together in much the same way that a WAN (wide area network, which will be defined later) does but over a smaller geographic area. The CAN typically connects LANs owned by a single company, university, government agency, etc.

### MAN

![Metropolitan Area Network city in the middle connected to several networks.](https://assets.wgu.edu/6c2f48013155eaeff55f8df5d09a108e)

Diagram. Metropolitan area network (MAN).

A metropolitan area network, or MAN, provides networking across a larger area than a CAN, but smaller than a WAN, such as a whole city or the equivalent of a metropolitan area (hence the name), though it is not necessarily limited by city boundaries. A MAN is made up of many LANs and is owned by many organizations, government entities, etc., within the city to create a fabric of network coverage, often at higher speeds than maybe commercially viable when connecting directly to a WAN when connecting to other entities in the same MAN. Often, this MAN is then connected to a larger WAN (usually the internet) for access beyond the city.

### WAN

![Wide Area Network: several computers connected around map of the earth.](https://assets.wgu.edu/c7c0af3ff1d59f2e73677736a352e3d7)

Diagram. Wide area network (WAN).

A wide area network, or WAN, is similar to a LAN, except that it covers a large geographical area within its network. This would be the case for worldwide businesses or government bodies. The internet is an example of a WAN, as it can connect individual users across the globe.

While the technical definition of a WAN is a network spanning a city, countries, or the entire earth, it is easier to think of WANs as a network that connects smaller networks, like LANs. WANs are able to link these smaller networks to transfer data over hundreds of thousands of miles, whereas a true LAN is only able to do so over its small network.

For example, banks use private WANs to connect hundreds of branches across the nation. This allows their sensitive user information to be passed from branch to branch without compromising security or traveling over a public network like the internet. Because of this, a banking customer can go to any branch across a country and have access to their accounts and funds.

In contrast to the above types of networking, there are two other ways of looking at networks: they are defined by who has the resources and who needs access to them.

### Client-Server

![All computers and laptops are connected via a single switch to the file server and directory server.](https://assets.wgu.edu/7ce8cfb8f6cc9b11ef6fb409f0e6afe1)

Diagram. Client-Server Network

In a client-server network model, there is a distinct server and a distinct client. The server is the system that stores data and information. The client is the machine that needs access to that data. This is the traditional model of networking since the 1990s.

### Peer-to-Peer

![4 computers in a peer-to-peer network connected to a single switch.](https://assets.wgu.edu/53f5e5df6087bc9af0f2b8e52cd79e4a)

Diagram. Peer-to-peer network.

In a peer-to-peer model, or P2P, there is no individually designated server or client. Each machine on the network can act as both server and client, sometimes requesting data from other nodes and sometimes answering requests from others. Bitcoin and Tor are examples of peer-to-peer networks.

### Bus Topology

![5 devices connected via a straight line in a bus configuration.](https://assets.wgu.edu/943418accc94b4b9bc71cfcef554719f)

Diagram. A bus network topology.

A bus network topology is a single line of devices connected together by one shared network cable. Though bus networks are typically drawn as a single straight line, the network cable is rarely as straight. Often the cable is passed around walls or cubicles so that each computer can be attached to the network.

Bus network topologies are uncommon today but were common in the early days of networking, before the advent of the Ethernet hub and switch. In a bus topology, computers connect to the network by physically tapping into the network cable using special adapters. This allows the network cable to remain one continuous conduit while also allowing the computers to send and receive electrical signals on the cable. This leads to an important requirement of bus networks: the ends of the cable must be properly terminated. At both ends of the network cable, special electrical resistors called terminators must be attached to absorb stray electrical signals on the wire. If these terminators are removed or if the network cable is accidentally cut, the electrical signals will not be properly absorbed and will bounce back along the wire, causing communication loss, a condition called signal reflection.

The network in a bus topology is also referred to as a network segment because the network may be extended by adding more segments of cable to either end of the network, allowing more computers to connect to the shared network. This may seem like a good idea but can have significant negative consequences.

Computers on bus networks communicate in half-duplex mode, meaning that you can either send or receive at any given time but cannot send and receive simultaneously. Also, the network cable in a bus topology is a shared communications medium, meaning that all computers attached to the network will receive any and all traffic sent on the network. You can visualize a one-lane road over a bridge, where cars must take turns traveling back and forth. This type of network performs well for a small number of computers but as it becomes more populated, it becomes exponentially more difficult to communicate with each other due to the collisions that occur when two or more computers attempt to transmit at the same time.

To better understand the implications of this shared one-lane medium, consider the following analogy of using walkie-talkie radios. You and your friend both have portable radios that share a common radiofrequency. You can either listen or speak, but not both. Your radio continuously receives whatever signals are sent over the air until you press and hold the transmit button, at which time you no longer hear what is being said on the radio and instead transmit your message. You and your friend may chat back and forth all day without problems, taking turns speaking and listening. Of course, you may have the occasional collision when you both try to talk at the same time, effectively garbling the transmission or cutting each other off. When it happens, you will clumsily have to pause and tell each other to go or wait and then restart your conversation. This is the same behavior that computers face on a shared one-lane medium. They must listen for a clear time to send their data or be faced with a collision that forces everyone to stop sending for a moment while the line clears. Now imagine that you add more people to the walkie-talkie analogy. The more people you have sharing that frequency, the more often you will have a collision and need to restart the conversation. The same is true when adding many computers to a bus network topology: it gets crowded very quickly.

Although a bus topology is very simple and usually inexpensive, overcrowding of devices can make the network unstable or unusable. And if the network cable is broken or cut, the entire network becomes unusable.

### Ring Topology

![5 computers connected in a circle or a ring on a blue background.](https://assets.wgu.edu/abee5aae0f320a87f024a4f2c7636a96)

Diagram: A ring network topology.

The ring topology was created to combat one of the more challenging aspects of the bus network: traffic collisions. As discussed in the previous section, when traffic collisions occur, all traffic must pause and wait for the line to clear before anyone can send again. This creates delays and degrades the performance of the network. To combat this problem, a ring network topology changes the way that computers know when to transmit and receive.

Imagine sitting around a campfire with children all talking at once. You have a stick in your hand and decide to call it the "talking token." You quiet everyone down and tell them that you will begin passing the talking token around the circle. You explain that only the person holding the talking token will be allowed to speak. Everyone else will listen. After saying a few words, the person with the token must pass it to the next person. No one can hang on to the token for very long. Everyone will have a turn holding the token, even if they have nothing to say to the group. This behavior can be found in computers running ring-based protocols such as token ring or fiber distributed data interface (FDDI). It allows the network cable to remain a shared medium, but it controls traffic.

Interestingly enough, ring topologies do not have to be physically arranged in a circle or even a ringlike shape. The network cable may run in a similar pattern to that of a bus network topology but with some important differences: the network cable is interrupted by each computer on the ring, and the cable is connected back to itself instead of using terminators. In a ring topology, the cable enters a “ring in” port on the network card of the computer and exits a “ring out” port on its way to the next computer in the ring. By definition, a ring is a closed-loop, and the ring topology is no exception. When building a ring topology, even if the computers are all physically arranged in a straight line, the network cable will always connect to itself. The cable exiting the “ring out” port on the last computer will be fed into the “ring in” port on the first computer, thereby closing the loop.

Ring topologies are generally more reliable than bus topologies. However, like a bus network, if the ring is broken, network communication will fail. In cases where the network must be highly available, a dual-ring topology can be used. In this case, there are two sets of cables, and each computer has two network cards, one for each ring. In the event of a single cable break, the second ring can take over, allowing network traffic to continue to flow. However, the dual-ring topology has its greatest benefit in the event that both rings are simultaneously cut. In this case, the two loose ends on either side of the cable break can be connected together, merging the two broken rings into one much larger, but continuous, ring, where traffic can flow. This dual-ring topology is commonly found in fiberoptic networks, such as the synchronous optical network (SONET) ring.

### Star Topology

![star topology shows desktop, laptop, database, connected directly with lines to middle device a network switch.](https://assets.wgu.edu/c1cb6a2f279e95a5e28981f2e34fe509)

Diagram. A star network topology with a central switch.

The star network topology, also known as a hub-and-spoke network, is an improvement upon the bus topology previously described. Unlike the single straight line of the bus topology, a star network is composed of a central network device, such as an Ethernet switch, connected to various network devices, such as servers, computers, and printers, by individual network cables. The name of the topology is derived from its shape in a network diagram. When drawn, the various lines connecting the switch to the network devices appear like the spokes of a wheel or the rays of light emanating from a star in the center.

In contrast to the other network topologies, where a network device such as a computer or printer is directly cabled (and therefore connected) to another adjacent device, in a star network, each device is only connected to the central switch. All device-to-device communication is sent through the switch at the center of the network and then forwarded by the switch to the proper destination.

Today, star networks are the most common type of network found in local area network (LAN) environments. For example, consider the network topology in a typical office where there are computers on each desk and a central wiring closet where servers and network switches may be stored. The desktop computers each have a network card that is connected to a network port on the wall. Behind the wall, the cable continues to run into and through the ceiling to the central wiring closet where all the other network cables in the office have been run. In the wiring closet, these network cables terminate at a patch panel with many network ports, each representing a location in the office where a wall outlet exists.

![Three computers connecting to phone jacks. Phone jacks connected to patch panel, which then connects to the switch.](https://assets.wgu.edu/87600e6fd87e22adf34483d42b21f34c)

Diagram. A patch panel.

When a computer is moved to a new location in the office, the network administrator can connect the appropriate network ports on the patch panel to a central Ethernet switch. The switch bridges the network traffic together and allows the devices to communicate with one another.

One key advantage of this topology is versatility. Instead of running cables from computer to computer, in a star topology, network cables are often run in the walls to a central closet. In fact, the owner of the building may decide to run many more network cables than are actually needed to anticipate future growth. This gives the network administrator the flexibility to move computers around the office without re-cabling the network. The owner must only connect the computer to the network outlet on the wall and then patch in the corresponding network cable to the central switch. This also means that a break in a single network cable will only impact one network device rather than the entire network. However, if the central switch fails, the network fails, resulting in loss of communication for all the devices in that network.

The star topology is not only used in LAN environments. It is also used in some forms of WAN, where many remote offices are connected to a central headquarters location. Each remote office then becomes a spoke off the hub of the central headquarters. When a computer in one remote office wishes to communicate with a computer in a different remote office, the traffic is passed through the central headquarters network. The star topology eliminates the need for a point-to-point network connection between each remote office.

### Mesh Topology

![5 computers connected to each other in a full mesh topology.](https://assets.wgu.edu/4328c6a8d33fe027137beb7314d508af)

Diagram. A mesh network topology.

The term mesh originates from the interconnected threads in a fabric or a net. Mesh topologies are often drawn as a web of direct connections between computers or nodes in a network. However, those connections may be permanent or constructed dynamically, as nodes need to talk to other nodes. A mesh topology permits nodes to communicate with each other; the topology may be either a full mesh, where every node has access to all other nodes, or a partial mesh network, where each node is only able to connect to a subset of the other nodes.

This may have you wondering how you would run cables for such a complex and dynamic network. Unlike other topologies such as bus, ring, or star, mesh topologies are not necessarily constructed using physical network cables. The nodes may connect using Wi-Fi or radio signals or by virtual links such as virtual private networks (VPNs). Another example of a mesh network is a collection of routers that are able to communicate with each other and learn the best path for traffic to take when passing from node to node in the mesh.

Mesh networks are typically used where communication within a network must be highly available and redundancy is needed. The nodes within a mesh network can communicate with each other, and these connections can be changed dynamically if one node were to fail. This behavior is often referred to as a self-healing network because the nodes in the mesh are aware of each other and can establish new connections around failed nodes as needed. Common use cases include wireless networks at home and in the office, as well as large collections of routers, such as on the internet.

### Centralization

In the early days of mainframe computers, nearly all computing and network power was centralized in a large data center. Users logged on to machines called dumb terminals to perform their tasks. They were so named because the terminal had no intelligence or sophistication to it. All the programming and functionality were contained in the mainframe; the dumb terminal just accepted user commands and rendered a display with the results. These dumb terminals were placed in offices and cubicles where users needed to work, whereas all the data was safely locked up inside the vault of a data center.

Even though mainframe computers are not used as much today, many resources are still centralized. For instance, strongly centralized web-based applications allow phones, tablets, and computers to behave like dumb terminals. The web browser on these devices does not perform the complex calculations or even store the data that are used within these apps. Instead, the computing and networking resources are hosted in a remote centralized data center, such as a corporate headquarters or a cloud data center. In some ways, cloud computing has allowed a strong centralization approach to make a comeback. You can perform the heavy processing in the cloud without concerns about the hardware of the user’s device.

![Server receives data from source. Server receives instructions from terminals and returns results to terminals.](https://assets.wgu.edu/3bcc28eb08759d7366a2221dd6db137d)

Diagram. Centralized network.

While security is a great benefit of centralization, it is not the only reason to centralize resources. By placing the computing and networking power in a central location, the owners and operators of the applications can better control the performance and availability of the applications. To help explain that point, think about a web-based application that is also available as a locally installed application on your phone. QuickBooks and Office 365 are two good examples, but there are many others. Imagine that you have an older phone, one that has no trouble opening web pages, but other applications just do not run as fast as they used to. You may favor the website version of Office rather than the installed version because it performs better on your phone. Here is what is going on behind the scenes. When accessing Office via the web browser, you are using a centralized web server farm that is running the application for you and just sending back the changes to the display. The performance is also much more constant and reliable, assuming that you have a good internet connection, because the application owners and operators have centralized their resources and can add more resources to their servers during periods of high demand, ultimately keeping the application running well and giving you a positive experience.

Now imagine that instead of using the web-based version of the application, you are using the locally installed version of that application. The performance of the application is based on the processing power of your hardware rather than servers in the cloud. This may allow you to use the application while you are disconnected from the network, but the application owners and operators cannot do much of anything to improve the performance of the application while it runs on your device.

### Decentralization

![One computer ethernet-attached to printer. Two computers are not network-connected.](https://assets.wgu.edu/794843ff65a47d1d49c32d97b553897e)

Diagram. Decentralized network.

On the opposite side of the spectrum lies decentralization, an approach that puts the computing power in the user’s device rather than a data center. In completely decentralized approaches to computing, there may not be a central data center at all and possibly no need for any of the users to even participate in a network.

Decentralization first became possible in IT when microcomputers were popularized by IBM in the 1980s. These machines could perform tasks without a central computer system to support them, which in turn enabled users to operate autonomously. Soon, challenges began to appear with this decentralized approach. To name just a few:

Users stored data in files on their cassette tapes or floppy disks before hard drives became reasonably priced, which often were not backed up or secured properly.

Mismanaged local security could allow data to fall into the wrong hands or even leave the organization on portable drives.

Data created by one user may have been incompatible with other users due to differences in operating systems, application versions, or even applications themselves, such as WordPerfect versus Word.

The benefits of decentralization can outweigh the disadvantages, though. Decentralized systems are able to operate without a network connection because their data and applications are available locally. This is ideal for portable systems more so than stationary desktop computers. Another advantage of decentralization is the lack of a single point of failure, or, perhaps more accurately, each computer is its own single point of failure because the computers do not rely on each other.

### Client/Server Model

![All computers and laptops are connected via a single switch to the file server and directory server.](https://assets.wgu.edu/7ce8cfb8f6cc9b11ef6fb409f0e6afe1)

Diagram. Client/Server Model.

The client/server model is very popular with enterprise applications such as email and databases, but client/server applications can be found in organizations of nearly any size. The name client/server alludes to the shared responsibility of the centralized server and the decentralized client computer that accesses the server. Client/server applications tend to store data in the centralized data center but may leverage the computing power of the user’s client computer to perform some tasks.

This approach offloads some of the computing requirements from the data center’s servers, but more importantly, the client/server model allows application designers to implement advanced user interfaces that would not otherwise be possible in a web-based or terminal-based application. In addition to the user interface, client software, unlike web browsers, usually has access to the hardware of the client computer. Consider the example of a client/server document scanning solution. The server-side software maintains the back-end database and image storage, while the front-end client software performs the scanning and data entry tasks.

There are still challenges with client/server applications. Though the data is stored centrally, the data entry and scanning are performed by the client computer. This could lead to data inconsistency issues if multiple users have the client software installed but they are running different versions of the client software. Additionally, client software is generally created for specific operating system versions, which may complicate future upgrades on the client computers.

### Peer-to-Peer Model

![4 computers in a peer-to-peer network connected to a single switch.](https://assets.wgu.edu/53f5e5df6087bc9af0f2b8e52cd79e4a)

Diagram. Peer-to-peer network.

Workgroups and very small companies may favor the simplicity of the peer-to-peer model for sharing data as opposed to creating a dedicated server. In a peer-to-peer network, client computers act as both servers and workstations because they share files and printers while allowing a user to log on and use the client computer for normal tasks. For example, consider a small network of four computers. The users have a collection of files they have been sharing via USB drive. The process of copying and pasting the files has become cumbersome and introduces delays in their work. They could, instead, choose to store the files on one computer and share them over the network in a peer-to-peer fashion.

Creating a peer-to-peer network is very easy. Most operating systems simplify this process by automatically discovering other computers with shared resources. In many cases, you can even automatically discover resources on different operating systems, which can be a big help if you have a mixed network of Microsoft Windows, Apple MacOS, and Linux.

Remember, the computer that will serve the files will perform double duty as a workstation and a server. When choosing the computer that will serve the files, select the least active computer or the most powerful computer in the group. This will minimize the performance impact of other computers accessing files on that computer.

### Wired versus Wireless Networks

![In a typical wireless network, computers are connected to a router by wifi. In a wired network, by cabling.](https://assets.wgu.edu/c3ec16ae3744923099a80f9edde69f26)

Diagram. Wired and wireless networks.

It is important to note that the network architecture does not depend on whether your network is wired, wireless, or a mixture of the two. You can operate a client/server network using wireless networking just as easily as you can with wired networks. The difference comes down to a couple of factors: portability versus stability.

Wireless networks are great for portability. You can take the computer wherever it is needed, as long as you have a wireless signal. The challenge is the strength and stability of that wireless signal. In some buildings, wireless signals may be intermittent, or you may encounter dead spots where the signal does not exist.

This is where wired networks excel. While you do not nearly have the degree of portability while connected to a wired network, you will have a very stable connection. In some cases, the bandwidth of a wired network may also exceed the bandwidth of the wireless network. However, take care not to assume that one connection type will always be faster. Wireless networking technology is constantly improving and may exceed the speed of some wired networks.

### Virtualization

Virtualization has been used in IT since the 1970s, when large mainframes and minicomputers needed to be logically divided into smaller virtualized computers to run workloads in isolation. Today, virtualization fulfills similar purposes, such as allowing one physical server to host many different virtual machines or to create network devices on demand, such as virtual routers and firewalls.

Virtual devices operate similarly to their physical counterparts but with a few differences and benefits. The very nature of these virtual devices practically gives administrators superpowers in the data center. Tasks that would be challenging or even impossible with physical devices now become commonplace, thanks to virtualization. For instance, you can do the following:

-   deploy new virtual devices quickly and on demand without the need to physically install new hardware move virtual devices within a data center or even between data centers without shipping or moving physical equipment
-   increase the reliability of an application or service by virtualizing it and separating it from hardware that may have once been a single point of failure (SPoF)
-   create point-in-time snapshots or clones of virtual devices for backup and recovery purposes
-   increase or decrease the compute, storage, and network resources allocated to a virtual device on demand as its utilization rises and falls

### Hypervisors

Virtualization relies on a special type of software, known as a hypervisor, which creates the virtual hardware for devices. There are many different varieties of hypervisors, including open source and commercial. Some hypervisors run as standalone applications on Windows, MacOS, or Linux, whereas other hypervisors are installed as the underlying operating system itself. Regardless, all hypervisors have something in common: they use software to create the illusion of physical hardware.

Hardware is essentially programming instructions baked into copper and silicon chips. With enough skill, you could recreate that programming in software. Now imagine that you learn how to recreate all the hardware in a computer’s motherboard as a series of software programs. You continue the process with its graphics card, network card, and even its hard drive. You now have a collection of programs that, when connected together, have the appearance of a physical computer, but it is executing as software. This is virtualization, and you have just created your first set of virtual hardware. Each instance of virtual hardware is called a virtual machine, or VM.

The virtual hardware is such an elaborate and convincing illusion that you can actually install a real operating system within the VM, and it works as if it had been installed on physical hardware. The operating system (OS) installed within the VM is often referred to as a guest OS to differentiate it from the operating system of the underlying physical computer, which is called the host OS. To help you remember these terms, just think of the hypervisor as a host to a number of house guests called VMs.

The hypervisor provides the VM, and therefore the guest OS, access to the physical CPU and RAM resources as well as access to a virtual disk that the guest OS believes is a real, physical hard drive. Optionally, you may also provide a virtual network card that also appears real and that will give the VM access to the network. With few exceptions, the guest OS will behave in the same way it would if it had been installed directly on physical hardware. To make the illusion complete, some hypervisors include special device drivers that you can install within the guest OS to gain performance improvements and access to features that would be otherwise impossible on physical hardware.

Hypervisors are able to host multiple VMs, each running its own guest OS and applications. Each VM has its own virtual hardware that the hypervisor manages and keeps isolated and independent of the other VMs. The hypervisor serves as a resource traffic cop in that it manages how each VM accesses and consumes the physical hardware resources, such as CPU, RAM, networking, and storage. To the rest of the world, these VMs appear as isolated and independent as individual physical servers. Also, despite the magic of virtualization, VMs still cannot communicate telepathically with one another. So, if you want them to talk to each other, you will have to install virtual network adapters in the VMs and configure their networking as you would do with your physical servers.

There are two types of hypervisors: Type 1 (bare metal) and Type 2 (hosted). Both types can host VMs; however, they have very different use cases. Type 2 hypervisors, which you will learn about first, look and feel like any other application that you may run on your laptop. Type 1 hypervisors typically requires dedicated hardware and are installed as that machine’s operating system, making them more commonly found in data centers than in home networks.

![Type 1 hypervisors are installed directly on a dedicated bare-metal server. Type 2 are installed on a host operating system.](https://assets.wgu.edu/c15cf48dd634cf40677393c6ada21302)

Diagram. Type 1 and Type 2 hypervisors.

#### Type 1 Hypervisors

Type 1 hypervisors, also called bare- metal hypervisors, differ from Type 2 hypervisors in the way they are installed. Remember that a Type 2 hypervisor, such as VMware Workstation, is installed as an application within your existing computer or laptop operating system. Type 1 hypervisors, such as VMware ESXi or the open-source KVM hypervisor, are operating systems that natively run virtual machines and are intended to be installed on a dedicated bare metal server. This is a significant difference because, as an operating system, the Type 1 hypervisor has complete access to the underlying hardware of the physical computer, which alleviates the performance penalty that Type 2 hypervisors commonly face.

Another important difference between the hypervisors is in how you access and manage the host and the guests. Type 1 hypervisors present very little information to the console screen of the host computer. While there may be a limited user interface for troubleshooting the hypervisor directly, all administration is typically performed from another computer, such as your laptop. On your laptop, you would direct a web browser to the IP address or hostname of the hypervisor to access its web-based administration portal.

To make this a bit clearer, consider the earlier example of using VMware Workstation to run a Windows Server VM on your laptop. The hypervisor was just an application installed on your Windows 10 laptop that you were logged in to and that was able to directly interact with the settings of Windows 10 (your laptop), VMware Workstation (the hypervisor), and Windows Server (the VM). Conversely, if you have installed a Type 1 hypervisor on a computer, you can see the basic troubleshooting interface on its monitor but must use a web browser on a separate computer to administer the hypervisor and the VMs running on it.

Also, remember that VMs are typically connected to the network just like any other physical computer. Users that need to connect to a VM typically are not granted access to the hypervisor configuration portal; rather, they are given an IP address or hostname for the VM that they need to connect to.

#### Type 2 Hypervisors

A Type 2 hypervisor, sometimes referred to as a hosted hypervisor, is installed as an application on personal computers or laptops. This allows the user to run different VMs that all share the laptop or computer’s hardware resources. This allows you to run operating systems within a VM other than what was natively installed on your computer or laptop. For instance, imagine that you are an application developer creating a new application that will run on Windows Server. Your laptop is running Windows 10, which is similar to Windows Server but may not be close enough for you to properly test your application. You could install a Type 2 hypervisor, such as VMware Workstation or Microsoft Hyper-V, to allow you to run VMs on your laptop. This would allow you to create a VM running Windows Server and then log in to the VM to install and test your application.

In another example, you are a student with a laptop running MacOS. One of your classes requires you to gain familiarity with Linux, but you do not want to purchase a second computer. Again, you could install a Type 2 hypervisor for MacOS, such as VMware Fusion or Parallels Desktop, which would allow you to create and run a Linux VM on your laptop.

One important aspect of Type 2 hypervisors is that they are installed and run as a regular application on your computer or laptop. This means two things: first, the hypervisor is competing for hardware resources with all the other running applications on your computer; and second, the hypervisor does not have direct and unrestricted access to the physical hardware but instead must send all your VM’s hardware requests through your computer’s operating system. Both issues can lead to degraded performance within your VMs, but slower performance may be far more desirable than buying and carrying around separate computers.

### Cloud Computing

![Some computers and devices are specifically networked together, some are not; but they are all connected to the cloud.](https://assets.wgu.edu/9f276c6c437b1b97284710b9c8687e12)

Diagram. Cloud computing.

Cloud computing may be the most commonly used term in IT, but if you ask an IT professional to define it, you will likely get the response, “It depends.” Pinpointing a single definition for cloud computing is difficult because it is many things to many people. Instead of trying to find one all-encompassing definition, consider the meaning and business implications for some of the more well-known and accepted characteristics of cloud computing: on-demand, self-service, resource pooling, elastic, accessible, and measurable.

Business owners and executives do not usually make impulse decisions about strategic direction, mergers and acquisitions, or massive marketing campaigns, but it can seem that way if IT is left out of the decision-making process. Implementing change takes time, and in the business world, time can cost you opportunities. Therefore, a quick reaction time within IT is critical to the success of the business. Without cloud computing, it may take weeks to acquire the necessary hardware, software, and manpower to satisfy the new business needs. The on-demand nature of cloud computing provides IT professionals the means to provision new servers, applications, and other resources in a self-service manner, often within minutes of the request.

Cloud providers, such as Amazon (AWS), Google (GCP), and Microsoft (Azure), purchase and manage vast quantities of compute, storage, and networking resources around the world. In doing so, they are able to pool these resources to achieve economies of scale, which can improve pricing and provide additional capacity to their customers for sudden bursts in their businesses. It is in this elasticity where cloud computing proves to be an immense business asset. Consider that you run a retail business with an e-commerce website. Most of the year, your website traffic is predictably average, but during the three months of the holiday shopping season, your website receives so much traffic that it occasionally crashes or performs so poorly that customers go elsewhere. What you need is a data center that can dynamically increase in size during the busy months and then shrink back down to size during the rest of the year. This elasticity, often referred to as scalability, is yet another key benefit of cloud providers. During your busy months, you could leverage the resources of a cloud provider to keep up with customer demand and then recede back to your own data center during the rest of the year.

Another reason cloud computing is so popular is the global reach that it provides companies. Consider again the retail business example. Imagine the business is located in a small town in the middle of the United States, but its products and services attract a global customer base. Currently, the business’s website is hosted in one location in the United States, which is great for U.S. customers, but the site is slow when accessed from Europe or Asia. To counter this problem, the company could leverage the global presence of cloud providers to host their website in data centers around the world. This improves their customer’s experience, which in turn may improve sales.

Finally, services in the cloud must be measurable. This alludes to the way that you pay for services in the cloud. Much like the way you pay for electricity or water at your home, cloud providers tend to charge you only for what you consume. This could be the number of hours that your virtual machines are running, the amount of data storage you have consumed, or even the number of gigabytes of network bandwidth that your customers consumed while browsing your website. So, just as you turn the lights off as you leave a room, do the same in the cloud. When not using resources, such as test or development systems, power them down and remove extra and unnecessary data. Of course, if you tend to leave the lights on, they will stay on, but you can expect a hefty bill at the end of the month. Ultimately, if you are conscientious about how you consume cloud resources, you will likely find cloud computing to be a very affordable alternative to traditional data centers.

Products and services within cloud computing are organized based on the type of service being offered and by the location where the service is hosted. The various types of cloud services are categorized by the cloud service models, whereas the hosting locations are classified by the cloud deployment models.

#### IaaS

You will start by learning about IaaS because it bears the closest resemblance to a corporate data center. First, you must understand the word infrastructure. In this context, infrastructure refers to the physical servers, storage, and networking that is required to exist before you can create any virtual servers or install any applications. This underlying infrastructure is maintained by the cloud provider so that you may focus your attention on the virtual machines and your applications. The cornerstones of the IaaS offering are server virtualization, storage virtualization, and network virtualization. Infrastructure as a service is very customizable, but it also means you are responsible for managing more things, such as the virtual machine configuration, its operating system, and all the patches that it requires.

With regard to server virtualization, the cloud provider manages the hypervisor and the underlying hardware. You, as the consumer, are given access to a web portal, which enables you to create virtual machines and customize their resources to fit your business and application needs. The cloud provider allows you to choose the number of CPUs, the amount of RAM, the amount of storage, and even the number of network cards in the VM.

Storage virtualization helps cloud providers offer you storage solutions that can expand in size or change in performance based on your business needs. When creating your VMs, you may be given the choice to provision regular storage at the normal price or very fast storage at a premium price. Your selection will depend on your application's requirements.

Network virtualization gives cloud providers the ability to create virtual private cloud (VPC) networks for each of their customers, keeping each VPC network isolated from the others. As a consumer, you may even create additional networks to isolate your virtual machines for testing or development purposes. Your VMs will use the VPC network to communicate with each other just like the physical computers in your data center use your internal network to communicate with each other. The VPC network may also have routers and firewalls that allow your VMs access to the internet or to other data centers around the world.

Server virtualization continues to play an important role in cloud computing, both for private clouds hosted within corporate data centers and for public clouds such as Google, Microsoft, and Amazon. Not only are virtual servers the flagship product offering in the infrastructure as a service (IaaS) cloud service model, virtual servers are also used by cloud providers behind the scenes to deliver their customer-facing platform as a service (PaaS) and software as a service (SaaS) products.

A word of caution is warranted here. The cloud provider typically has little to no interaction with your virtual machines, leaving you with the responsibility to protect them from disaster (via replication) and data loss (via regular backups). In the event that one of the cloud provider's physical servers were to fail, the cloud provider is responsible for repairing their equipment; however, depending on your support agreement with the cloud provider, they may or may not be financially liable to you for the outage or responsible for restarting your virtual server following the outage.

Also, keep in mind that in most legal jurisdictions, the cloud provider is not obligated to automatically back up your data, keep archive copies of your data, or even move your data to another location without your express consent and direction. This is not much different than deploying a VM in your own home lab environment. It is not automatically backed up or replicated to another location. If you suffer a hardware failure, you lose the VM. The principle advantages of IaaS solutions are that you can customize the infrastructure to suit your needs, install nearly any application in your VMs, and, if desired, implement high availability and backups for your solution. When deploying a production application to the cloud, build redundancy and disaster recovery into your design by deploying at least two of everything: one instance in a nearby data center for production use, and one instance in a geographically distant data center for safekeeping.

#### PaaS

If you just need a platform on which to deploy your application or you simply need a database without the hassle of managing the server, PaaS makes this easy. In PaaS solutions, the cloud provider is responsible for the virtual servers and, in some cases, the services that run on top of them, such as a database engine, and provides you with a platform on which you can run your code or store your data.

You may have seen or heard about PaaS services in the past and yet not realized it because cloud providers rarely label their services as IaaS, PaaS, or SaaS. One example of a PaaS offering is basic web hosting, a service that has been around since the dawn of the web. Web hosting, like all PaaS offerings, is a partially managed service. The provider gives you limited control over a web server that they maintain for you. You have the ability to log in and upload your code, but they maintain the server for you, including the virtual hardware, guest OS, web services, and the patching for the OS and web services.

PaaS solutions are particularly attractive for application developers because it allows them to deploy their code to an application runtime environment, such as Java, .NET, or Node.js, that is backed by an ambiguous pool of compute resources. That may sound magical, but the cloud provider's goal is to abstract the details of the resource consumption away from the application code and allow the application to scale up and down based on its load, such as the number of people using the application, or the amount of data the application is processing.

A branch of PaaS solutions designed to further simplify the deployment of application code has gained so much popularity that it has been given its own name: serverless computing. The term serverless is not intended to imply that there are no servers, but rather that the consumer of the service (the developer in this case) typically is not even made aware of the number of servers being used in the back end to run the application. These solutions are also gaining in popularity because they can quickly deploy and then scale new applications with minimal effort required by the IT operations team, thereby increasing the reaction time of IT to changing business needs.

#### SaaS

SaaS solutions, like PaaS solutions, are often overlooked because they are so ubiquitous. The term software in SaaS could represent nearly anything you consume over the internet. A few examples include social media (Facebook), word processing (Office 365), and a line of business applications (Salesforce). Even now, you are using an SaaS solution to view this course and read this text. Software as a service allows consumers to store and potentially publish information without the need to manage the underlying applications or infrastructure.

#### Private Cloud

The term private cloud is most often associated with equipment hosted within a single company’s on-premises data center. The company purchases or leases the computer, storage, and networking hardware and maintains the data center facilities. If a failure occurs, the company is responsible for repairing the problem themselves because all the equipment belongs to and is managed by them.

It is possible to have a private cloud that is not hosted within the company’s data center. The company may lease space in a commercial data center and operate the equipment there. This is usually referred to as co-locating, or a "co-lo" solution, because the company is co-locating its equipment with the commercial data center’s equipment. Some public cloud providers also offer this as an option for customers who require complete control over the physical equipment yet wish to house the equipment outside their own data center.

The primary advantage of a private cloud is the ownership and control that a company has over the equipment. Some companies use a private cloud only because of regulatory restrictions that mandate the company to maintain absolute control over the hardware and software that run a particular system.

#### Public Cloud

There are many public cloud providers, but some providers, such as Amazon Web Services (AWS), Microsoft Azure, or Google Cloud Platform (GCP), are more well-known because of their marketing and experience in the industry. As with "private cloud," the term "public cloud" refers to the ownership and maintenance of the underlying infrastructure and facilities. In the case of a public cloud, the cloud provider is responsible for maintaining the hardware and repairing the infrastructure instead of the customer.

Another common misconception is that public cloud providers are inherently insecure because they host content from many different companies; however, the opposite is much more likely to be true. Public cloud providers must keep their customers’ data isolated from one another and must follow strict rules that govern how data is handled and destroyed. Even their physical data centers are required to have the most state-of-the-art security available. In some cases, public cloud providers may have a higher level of security than the customers they host.

Another consideration is the concept of multi-tenancy, meaning when multiple tenants share the same physical resource. In any multi-tenant situation, there are potential security and performance implications because you are sharing hardware with other companies, though the risks may not be as significant as they seem. Multi-tenancy in computers is analogous to living in an apartment building. Many different people live within the same apartment building (the physical computer), but each tenant (the customer) has their own apartment (a VPC) with a lock on the front door (a firewall). In addition, for extra privacy, the members of a tenant’s family (the servers of one customer) may even have their own rooms with locked doors to further isolate themselves.

#### Community Cloud

Community clouds are uncommon in the commercial sector but may be found in universities or government agencies. These clouds are data centers that are jointly owned and operated by the tenants. Think of it as a semi-private cloud for each tenant, with the added benefit that the maintenance and management of the underlying infrastructure is shared by all the tenants.

#### Hybrid Cloud

The term hybrid cloud refers to a combination of private cloud and public cloud and is most commonly associated with companies that extend their applications and services between their own data center and that of a public cloud provider's. This may be done to allow the company easy access to additional computing resources during times of burst demand, or as a way to host most of their services in the public cloud with the exception of the few applications that are subject to regulatory controls and must remain at an on-premises data center.

For hybrid cloud computing, the customer will require a dedicated connection between their on-premises data center and the public cloud provider. This connection may be a virtual private network (VPN) established over the internet or a dedicated wide area network (WAN) connection maintained by a telecommunications provider.

#### Multi-Cloud

Multi-cloud is the concept of leveraging the services of multiple public cloud providers, such as hosting your website at AWS and GCP and balancing the users between these providers. This concept, in practice, can add redundancy and flexibility.

Another use case is when a company currently uses services in one cloud provider but another cloud provider excels or provides cheaper services in a particular area, for example, machine learning or data warehousing.