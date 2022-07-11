![A network firewall serves as a metaphorical wall, dividing computers in a LAN from those in the WAN.](https://assets.wgu.edu/284e633988bbaee9fc9c9b4cbb5ccd26)

Diagram. Firewall.

### Firewalls

A network firewall is a barrier that intercepts and inspects traffic moving from one area of the network to another. Nearly all networks today benefit from the protection of some type of firewall. In all likelihood, you passed through several firewalls when you opened this material. You probably have a firewall at home that allows you to access the internet while simultaneously preventing intruders from accessing your home network. The servers hosting this material are also protected by a firewall that limits the type of internet traffic that can reach them.

Firewalls come in a variety of forms and provide a range of functionality. Some may be physical appliances mounted in data centers, while others may be virtual appliances operating as VMs (virtual machines). Still, there are others known as host-based firewalls that operate as applications running on workstations and servers. They all have something in common though; they have a set of rules that define whether the firewall will permit or deny the traffic to pass on to its intended destination. In the following sections you will explore firewall types, functionality, and terminology.

![Diagram depicts 7 layer OSI network filtering model, packet filtering occurs at Layer 3 (Network) and Layer 4 (Transport)](https://assets.wgu.edu/18a36066ff38960df6011e3654a882b7)

Diagram. Packet filtering in the OSI model.

### Packet Filters

A packet filter is a firewall that operates at Layers 3 and 4 of the OSI network model: network and transport.

In most networks today, that equates to the IP address (Layer 3) and the TCP or UDP port number (Layer 4) of the traffic passing through the firewall. These firewalls inspect incoming (ingress) and outgoing (egress) traffic and compare the following attributes to a database of packet filter rules that determine if the firewall will forward (allow) or drop (deny) the traffic:

-   Protocol (typically IP)
-   Source IP Address
-   Destination IP Address
-   Source TCP or UDP port number
-   Destination TCP or UDP port number

These firewalls are only concerned with the address label (header) of the packets and perform no level of inspection on the contents of the packet (the payload). This means that potentially dangerous payloads could pass through a packet filter without being detected as long as the source and destination values were approved by the firewall rules.

### Circuit-Level Gateways

A circuit-level gateway is a device that operates as a middleman between two or more systems to help conceal the true identity of the client and server. The gateway may change the IP address and the TCP/UDP port number of the traffic to allow two networks to communicate that otherwise could not (for example, your home network and the internet).

Circuit-level gateways are the foundation of network address translation (NAT) and port address translation (PAT), which are commonly used in firewalls to allow private IP address ranges to communicate on the internet. These firewalls are only concerned with the address label (header) of the packets and perform no level of inspection on the contents of the packet (the payload). This means that potentially dangerous payloads could pass through a packet filter without being detected as long as the source and destination values were approved by the firewall rules.

![In the 7-layer OSI model, a Stateful Firewall is at Layers 3 (Network), 4 (Transport), and 5 (Session).](https://assets.wgu.edu/f89880a8dfb34f836f2f300fed3872bf)

Diagram. A stateful firewall in the OSI model.

### Stateful Inspection

To help you understand the significance of stateful inspection in firewalls, you must first understand the meaning of the term state. In this context, the word state refers to the connection state of a conversation between two computers. Some protocols, such as TCP, require that the recipient of a message respond back to the sender with an acknowledgment that it received the data. In a packet filter firewall, this would require at least two firewall rules: one that allows the sender to transmit data to the recipient, and another that allows the recipient to respond (acknowledge) back to the sender. Now consider the implications of a sender communicating with many recipients. There is still one rule for the sender, but now there are many rules for the acknowledgments because each recipient requires a rule to respond to the sender.

To reduce the number of firewall rules needed to support TCP communication, firewall vendors implemented a feature known as stateful inspection. This feature allows a firewall to identify traffic as conversational and automatically create temporary firewall rules to permit the response traffic to flow back to the sender. In this way, instead of maintaining a multitude of rules, in a firewall with stateful inspection, you only need to create a firewall rule that allows the communication to begin.

### Application Level

Remember, packet filter firewalls lack the ability to inspect the contents of the packets. Because of this, malicious traffic could pass into the network unchecked. To combat this potential weakness in security, network administrators began using proxy servers that could act as a middleman, reading and parsing the traffic payload, and then forwarding it on to the intended destination if the payload was safe. This behavior was later incorporated into firewalls to provide a deeper level of inspection. Firewalls with this ability are commonly called application-aware firewalls, or Layer-7 firewalls because application is the seventh layer of the OSI model. 

### Intrusion Detection and Prevention

Intrusion detection systems (IDS) and intrusion prevention systems (IPS) are advanced security solutions that can identify malicious traffic based on a database of known behaviors and payload signatures. IDSs monitor the network to detect threats, whereas IPSs intercept and block threats.

Both types of systems can be configured to operate in tap mode, which is where they attach to the network as listening devices only. The name tap comes from the term wiretapping because these devices are essentially eavesdropping on the traffic flowing through the network. The tap mode works well for IDS devices because they are passive listeners on the network and are designed to alert a network administrator if they detect any suspicious behavior.

On the other hand, tap mode does not work as well for IPS devices, which are designed to intercept and block suspicious traffic. For an IPS device to stop traffic, it must be positioned in the middle of the traffic stream, a configuration known as in-line mode. Typically, IPS devices have many network ports that are designed to operate as input/output pairs. The network administrator will physically route cables through the IPS device to create choke points in the network. For example, you have a set of public web servers connected to a dedicated network switch that is connected to your firewall by one network cable. You acquire an IPS device so that you can scan the traffic entering and leaving that network. To do so, you will disconnect the existing cable that connects the switch to the firewall and then place the IPS device in-line by connecting the firewall to one of the ports in an input/output pair and the switch to the other port in the pair. The IPS device bridges the traffic and appears invisible on the network, yet it is actually inspecting every packet and copying it from one cable to the other.

If the IPS device detects an anomaly, such as an unknown packet type or pattern of traffic, it can alert the administrator or block the traffic immediately. If it detects malicious traffic, it typically blocks the traffic automatically. There are also cases where the IPS device may block traffic, particularly files that are known to carry viruses and malware. This is a method known as reputation-based protection, because the file is blocked based on how often that type of file is found to carry viruses or malware. A good example of this is when IPS devices and firewalls block executable (EXE) attachments or downloads.

Like firewalls, IPS and IDS devices are not always physical appliances. They are also available as virtual appliances and as host-based IPS/IDS applications, which can be installed on your servers or workstations.

![The IDS allows read only access between local network and firewall.](https://assets.wgu.edu/d9ace8bd3baa8d9f9c4defdb68fd973f)

Diagram. Intrusion detection system (IDS).