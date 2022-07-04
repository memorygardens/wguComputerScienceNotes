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