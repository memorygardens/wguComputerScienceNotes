# Network Security Terminology
### _Asset_: 
A person, device, location, or information that SecOps aims to protect from attack.

### _Attack_:
An action taken by a threat that exploits a vulnerability that attempts to either block authorized access to an asset, or to gain unauthorized access to an asset.

### _Risk_:
The potential of a threat to exploit a vulnerability via an attack.

### _SecOps_:
The abbreviation for IT security operations; a discipline within IT responsible for protecting assets by reducing the risk of attacks.

 ### _Threat_:
Something or someone that can exploit a vulnerability to attack an asset.

### _Vulnerability_:
A weakness in software, hardware, facilities, or humans that can be exploited by a threat.

### Vulnerability Testers

As the name suggests, a vulnerability tester is responsible for scanning servers and network devices for known vulnerabilities. There are a variety of vulnerability scanning tools on the market. Some are open source, such as Nessus, whereas most are commercial products.

Typically, vulnerability testers are the good guys, though hackers also play a similar role, which attempts to find new vulnerabilities in software that can be exploited.

### Blue, Red, White, and Purple Teams

If you really want to know how well your security can withstand an attack, add some friendly competition. The terms _red team_ and _blue team_ originated in the military. The red team attempts to compromise the security, while the blue team defends. There may also be a neutral white team that observes the festivities and may even serve as referee.

Some companies use this attack and defend approach but take it to the next level by involving continuous improvement in the process. This is referred to as purple team (remember that red and blue together make purple). In the purple team approach, the red and blue team engage, and then when certain success criteria are met, the teams debrief, cross-train each other, and repeat. This is also known as an iterate and improve model.

### Hackers: White Hat, Black Hat, and Gray Hat

If you have ever seen an old western movie or TV show, you may immediately recognize this reference to hat colors. In those shows, the bad guys typically wore black hats, while the good guys wore white hats. Fast forward to today: we now use the terms black hat, white hat, and even gray hat to describe InfoSec hackers and their intentions or ethical position.

White hat hackers are IT professionals who specialize in penetrating or compromising network security but only to help an organization improve its own security posture. Most importantly, they only perform the attacks when authorized to do so; to the fullest extent possible, they remain in compliance with any and all laws governing such behavior.

Black hat hackers, on the other hand, may or may not be IT professionals but possess the knowledge and will to breach systems for profit. That profit may be monetary, street credibility, or just a source of entertainment. Black hat hackers do not ask permission and are not interested in helping their targets improve their network security.

In the middle of the spectrum are gray hat hackers, a group of people who may or may not be IT professionals and may or may not choose to break laws in pursuit of their hacking goals. Unlike black hat hackers, gray hats have no malicious intent in their actions; unlike white hats, they may not have obtained permission to perform the attack.

### Insider Threats

Some of the most potent threats come from people within your organization. Because they have legitimate access to systems, they are in a position to hack from the inside of the network, often undetected. Furthermore, a disgruntled insider may have a motive. Whenever you combine motive and opportunity, you have a substantially increased risk of trouble.

But not all insider threats are malicious in nature. Accidents happen, and if your account was granted extraordinary privileges, you could accidentally impact a large number of users with a single incorrect command. In both cases, the key to success is restricting access to the minimum set of permissions needed to perform the job and enable audit logging of all administrative actions so that you can later determine the cause of mysterious changes.

### Nation States

Industrial espionage is not just a theme for movies, it happens in real life on the internet. In a global economy, knowledge is power. Knowledge takes on many forms but is usually based on data or designs that companies refer to as intellectual property.

Consider an example of a fictitious country called Atlantica, positioned in the middle of the North Atlantic Ocean. Atlantica has a large labor force but almost no high-tech industry. Companies from wealthier countries have been building factories in Atlantica to take advantage of the inexpensive labor but have refused to share their intellectual property with other native Atlantica companies. Atlantica develops a plan to steal the intellectual property by hacking these more advanced companies so it can acquire the knowledge and designs it needs to kick out the foreign companies and produce the products itself.

While the example is extreme and perhaps unlikely, intellectual property theft through industrial espionage is a very real concern for many companies. The bigger threat is that _nation states_ have substantially larger budgets to hire hackers than the average criminal enterprise.

### Script Kiddies

Script kiddies are the copycat criminals of the hacking community. They typically hack out of pure curiosity or entertainment and often use poorly documented tools or scripts written by much more advanced hackers. Script kiddies have no formal InfoSec training and are typically not IT professionals. It is this lack of knowledge that contributes to the unpredictability of their actions and the random levels of damage that results from their attacks.

Also, contrary to the name, script kiddies are typically not kids at all; they may be adults who recently learned a thing or two about security and now wish to try things out in the real world, not realizing the consequences of their actions.

# Common Threat Attacks
### Wiretapping

This term comes from a historical technique used to spy on telephone calls. At the time, telephones transmitted analog electrical signals over copper wires that ultimately led to the telephone company. If an eavesdropper knew which wires belonged to a particular home or office, they could use a special telephone handset equipped with wire clips, or "taps," to listen in on the call. The process of clipping the taps to the telephone wires became known colloquially as "wiretapping"; today, it refers to any process that allows an attacker to electronically eavesdrop on a conversation, whether between two humans or two computers.

This form of attack can also include putting special wiretaps in-line with a computer’s network cable and then using a device called a "packet sniffer" to listen and record the traffic on the network. Alternatively, the attacker may put the wiretap in the wall behind a network jack. Wiretaps often use a wireless transmitter to send its ill-gotten information to the attacker’s computer. In cases where the security team might notice the attacker disconnecting the target device to add the wiretap, an attacker could use a special listening tool that interprets the electromagnetic field (EMF) surrounding a network cable so that the attacker can eavesdrop on a wire without even breaking its connection. To combat this problem, some organizations exclusively use fiber optic cables in their high-security areas. Though fiber optic cables are not immune to all wiretapping attacks, they are immune to EMF listening devices because fiber optic cables use photons (light) instead of electrons to transmit information.

### Port Scanning

When planning an attack, the attacker needs to know what type of services or applications are running on the victim’s computer. Fortunately for the attacker, this is easy because most network-accessible services open TCP ports to accept connections from legitimate client computers. An attacker just needs to send traffic to each and every port to learn which services are running. Unfortunately for the attacker, there are tens of thousands of ports, numbered from 0 to 65,535.

It was not long before tools made this job easier. An application called a "port scanner" can systematically check each of these ports by sending thousands of TCP/IP packets to the victim’s computer, each packet on a different TCP port. The victim’s computer will discard requests made to ports that are not assigned to a running application or service. The port scanner is then able to see which ports respond and which do not, allowing the attacker to perform more in-depth scanning to determine what service is running and if there are any known vulnerabilities present in that service.

### Taking Control

Once the attacker knows which ports are accepting traffic, the attacker can run standard vulnerability scanners against the victim’s computer to learn if any of the services can be easily exploited. This is yet another reason why you should routinely use a vulnerability scanner against your own servers. Even if you do not, attackers will.

Database servers are a popular target of attacks because they typically contain high-value information. But, more importantly, vulnerabilities are often found in applications that allow users to query databases. A particularly well-known attack called a SQL injection allows an attacker to take control of a database server by inserting special commands into input boxes instead of entering basic text. For example, you may have an application that allows a user to search for products by keyword. The application has a form that reads the keyword and then adds it to a Structured Query Language (SQL) command that is executed by the database server. So, instead of entering regular text, the user or attacker enters a specially crafted string of text that includes SQL commands designed to take control of the server. In a perfect world, the developer of the application would include code that validates the text that the user typed and would discard it if anything other than text was found. Unfortunately, there are many applications that do not check the input carefully and end up running nefarious SQL commands that compromise the security of the database server.

Another popular attack vector is a buffer overflow. Much like the SQL injection attack, this attack is made possible by applications that do not properly validate user input for extraneous content. In this case, the attacker purposefully enters text that is too large to fit within a region of memory called a "buffer." By entering more characters into the buffer than it can handle, some of those characters will overwrite neighboring, potentially executable areas of memory. This is not a regular or even random string of characters, though; it is compiled code that contains executable instructions that will grant the attacker control of the server. Under normal circumstances, the CPU of the server would simply ignore the compiled instructions; however, if the attacker correctly guesses the exact size of the memory buffer, the attacker can overflow it and trick the CPU into executing the rogue instructions.

There are two main protections against these attacks. The first is to review your source code and verify that all user input fields are checked for robust or unplanned values. Second, enable the NX-bit (no-execute) functionality on the physical computer or VM to tag memory buffers as containing storage (data) or CPU instructions (code). With the NX-bit enabled, the CPU will only execute the contents of memory buffers identified as code.

### Spoofing

Hacking a server and taking control of it may get noticed quickly, so attackers may prefer the more subtle approach of eavesdropping to gain the information they desire. Unfortunately for the attacker, eavesdropping is becoming much more difficult due to advances in networking, such as the Ethernet switch. To gain access to the information, the attacker needs to get into the middle of the conversation; however, to do so, the attacker must impersonate the sender and receiver of the traffic. This act is known as "spoofing its identity."

Consider as an example a man-in-the-middle attack. An attacker wants to intercept the communication between a client computer (client) and a server. The attacker will likely use two network interfaces, one that is spoofed to look like the server and another to look like the client. When the real client attempts to contact the server, the attacker’s computer responds to the client and captures the request. The attacker then replays that connection request from their computer using the network interface that has been spoofed to appear as the client. The server exchanges information with the attacker believing the attacker is the client, and then the attacker forwards the response back to the actual client so that no one notices the break in connection. There are many variants of spoofing. Another example involves ARP poisoning, which is a method attackers use to cause an Ethernet switch to flood all traffic to every port on the switch, including the attacker’s computer.

### Denial-of-Service (DOS)

Threats are not restricted to data loss or gaining unauthorized access to data. There are also threats that make data or entire systems unavailable to anyone. Threats known as denial-of-service (DoS) attacks do just that: they deny someone access to a service, usually by overwhelming the victim with enormous amounts of useless traffic.

Many DoS attacks use features within the ICMP, such as "ping." You may recall that ping is a tool commonly used by network administrators to verify that a computer is online. When you ping a computer, your computer sends the remote computer an ICMP echo-request packet, which essentially asks the remote computer to reply back to you. When the remote computer receives the echo-request packet, it automatically responds back to the source address with an ICMP echo-reply packet. Herein lies the problem: attackers learned that they could forge the source address of the echo-request, making the target computer believe the request came from another location and correspondingly send its echo-reply packets to another computer rather than the attacker. This redirection allows the attacker to continue attacking with minimal stress on the attacker's computer.

This opened the door for a number of attacks, some of which no longer function due to fixes made within the TCP/IP network stack on modern computers and routers. The first was the ping of death, a trick whereby the attacker would send the victim a malformed ICMP packet that would cause the victim’s computer to crash or stop functioning on the network. After the ping of death was patched, a new attack called the "ping flood" took its place.

The ping flood attack overwhelms a victim’s computer with an immense volume of ICMP echo-request packets, all containing a forged, randomized source address. The victim’s computer automatically begins sending ICMP echo-reply packets to all these forged source addresses, which eventually overwhelms the victim’s computer so that it cannot do its normal job. Fortunately, even though the source address is forged, this type of attack typically can be stopped and sometimes even prevented. Its big brother, the "Smurf attack," however, is significantly more difficult to stop and prevent.

The Smurf attack is a distributed denial-of-service (DDoS) attack, which means that instead of one computer sending forged packets to a victim, in the Smurf attack potentially thousands of computers will bombard the victim. The difference is subtle but important. In the ping flood, the attacker sends an ICMP echo-request with a forged source address to the victim, forcing it to send a corresponding echo-reply packet to a random computer. In the Smurf attack, the attacker sends a forged ICMP echo-request packet to the broadcast address of a large IP subnet, which means that a massive number of computers would all receive the message. Instead of randomizing the source address as in the ping flood attack, in the Smurf attack, the attacker specifies the victim’s address as the source address. As each of the hundreds or thousands of computers receives the ICMP echo-request packet, each will respond by sending an ICMP echo-reply packet to the victim’s address, thereby crippling its network connection.

There are also other DDoS attacks that aim to exhaust a computer’s CPU or network connections, including SSL attacks, which cause the victim’s computer to consume excessive CPU time as it constantly sets up and tears down thousands of SSL encryption sessions over and over.

### Social Engineering

Trust is a weakness, at least in the InfoSec world. It is usually substantially easier to "hack a human" than hack a computer because people are generally trusting of others. This leads to a class of attack known as "social engineering," the art of manipulating human trust to gain access or information. Here are some examples.

-   Impersonation:
    -   You overlook or just do not report the person resembling an electrician who is working on a nearby wall outlet. (He is actually installing listening devices on your network cables.)
    -   The helpdesk resets a user's password over the phone without being able to recognize the person's voice. (It was an imposter who can now log in as that user.)
    -   You hold the door open for a man dressed in a courier's outfit who seems to be carrying very heavy boxes into the office. (The boxes contain his computer and additional hacking tools.)
-   Phishing:
    -   You answer phone or email surveys or sales calls that discuss the type or brand of your security devices or policies. (They were assessing your security posture and checking how difficult your defenses would be to overcome.)
    -   You click links in emails from the IT department asking you to test a new web-based email that of course requires you to log in. (The email was fake and the web page is a phishing site that collects usernames and passwords.)
    -   You accept that free USB drive from a new vendor and plug it into your computer. (The drive contains a stealth phishing tool that reports your keystrokes back to the hacker.)

# Risk Mitigation
### Honeypot

A honeypot is a server or device that is configured to look very authentic, potentially containing data that appears to be legitimate user data, or configuration files that seem authentic. It is also known as a "tar pit" because it is intended to attract or distract would-be attackers from the actual targets on the network. The goal of the honeypot is to provide a false positive for hackers, whereby the attacker breaches the honeypot and believes the data it contains is the target’s actual data.

An alternate use of the honeypot or tar pit servers is to collect data on the attacker. A tar pit server is similar to a honeypot in that it contains data that is fictitious; however, the tar pit server is also designed to slow down the attacker so that tracing information can be obtained by the intrusion detection system (IDS).

### Proactive and Preventive Measures

Think about the number of threats and attacks discussed in this course. Aside from powering off your computers, it is difficult to imagine a solution that could protect a network from all the possible attacks and attackers. Security is not a task that you check off on a list, but rather a constant process to be performed. It is like a perpetual game of cat and mouse.

To combat these problems you need to take an in-depth defense approach to network security. That means you will use multiple tools and methods together in an overlapping manner to create rings or layers of security. If one component is compromised, there should be at least one other obstacle to overcome before the attacker gains access to the system. Ideally, you will mix different methods of defense, such as using an application-aware firewall on the perimeter and then relying on an intrusion prevention system (IPS) within the network and firewall and anti-malware software on the servers.

Minimize your exposure by keeping your operating systems and applications up to date on patches. Additionally, follow security-hardening guides that help you remove unnecessary services and features that may be susceptible to attack.

### Risk Mitigation Response

If a virus is spreading throughout the network, you will not have time to develop a plan and then act on it. So, be sure to develop and test your containment plans before an attack occurs. The response plan should first help contain the damage from the attack, which may involve quarantining computers or severing network connections, and then work to remove the threat and clean up the damage.

Remember that some attacks are silent and may not cause obvious damage right away. Such is the case with rootkits, backdoor attacks, and Trojan horses. Run complete antivirus and anti-malware scans on your systems regularly and keep the virus definitions as up-to-date as possible to help you detect new and emerging threats.