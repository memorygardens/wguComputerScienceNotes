![[Pasted image 20220627222905.png]]

### TCP/IP
![[Pasted image 20220627224841.png]]
**TCP/IP** stands for transmission control protocol/internet protocol and is a set of protocols used to connect network devices to each other.

**The TCP/IP networking model is made up of four layers:**

1.  Application Layer: This layer is responsible for the communication protocols between nodes. The protocols in this layer include hypertext transfer protocol (HTTP and HTTPS), Secure Shell (SSH), and network time protocol (NTP), among many others.
2.  Transport Layer: This layer is responsible for the end-to-end transport of data. The protocols that live in this layer are transmission control protocol (TCP) and user datagram protocol (UDP).
3.  Network Layer: This layer defines the logical transmission protocols for the whole network. The main protocols that live in this layer are internet protocol (IP), internet control message protocol (ICMP), and address resolution protocol (ARP).
4.  Network Interface Layer: This layer establishes how data should be physically sent through the network.

The TCP/IP model is used for practical application when locating specific protocol. It covers the same topics that will be found in the OSI model but in fewer layers.

### OSI Model 
![[Pasted image 20220627225119.png]]

**The OSI** (Open System Interconnection) model consists of a seven-layer architecture that organizes the sending of data from hosts across a network. The OSI model was developed by the International Standards Organization (ISO) after the TCP/IP model to provide greater granularity of networking assignments within the model.

**The layers are:**

1.  Physical Layer: This layer is responsible for the physical connections of the devices in the network. This layer is implemented through the use of devices such as hubs, repeaters, modem devices, and physical cabling.
2.  Data Link Layer: This layer is responsible for the error-free delivery of data to the receiving device or node. This layer is implemented through the use of devices such as switches and bridge devices, as well as anything with a network interface, like wireless or wired network cards.
3.  Network Layer: This layer is responsible for the transmission of data between hosts in different networks as well as routing of data packets. This layer is implemented through the use of devices such as routers and some switches.
4.  Transport Layer: This layer provides services to the application layer and receives services from the network layer. It is responsible for the reliable delivery of data. It segments and reassembles data in the correct order for it to be sent to the receiving device. It may also handle the reliable delivery of data and any retries of data that are lost or corrupted (for example, TCP does this). This layer is often called the heart of OSI.
5.  Session Layer: This layer is responsible for connection establishment, session maintenance, and authentication.
6.  Presentation Layer: This layer is responsible for translating data from the application layer into the format required to transmit the data over the network as well as encrypting the data for security if encryption is used.
7.  Application Layer: This layer is responsible for network applications (like HTTP or FTP) and their production of data to be transferred over the network.

The OSI model is widely used throughout networking documentation and discussions. Layers are often referred to by number, not name, so memorizing the numbers and having a good understanding of each layer’s uses are essential for success in the IT community.

![[Pasted image 20220627231627.png]]

# Model Comparison 
![[Pasted image 20220627231954.png]]


