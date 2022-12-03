# `Networking Notes`

## What is Networking ?

>Networks are simply things connected. In computing, a network can be formed by anywhere from 2 devices to billions. 

## What is Internet ? 
> The Internet is one giant network that consists of many, many small networks within itself.
 
![image](https://assets.tryhackme.com/additional/networking-fundamentals/intro-to-networking/what-is-the-internet/internet2.png)

>There are 2 types of Networks:
1. Private Network  
2. Public Network

>As previously stated, the Internet is made up of many small networks all joined together.  These small networks are called private networks, where networks connecting these small networks are called public networks.

>Public IP addresses are given by your Internet Service Provider (or ISP) at a monthly fee (your bill!)

## What is IP Address?
>An IP address is a set of numbers that are divided into four octets. The value of each octet will summarise to be the IP address of the device on the network.

![octets](https://user-images.githubusercontent.com/35003220/205220342-8452cc41-78b0-4feb-b7c7-e4547c9b9b18.png)

>Older one is an IPv4 addressing scheme, which uses a numbering system of 2^32 IP adresses (4.29 billion)

>IPv6 is a new iteration of the Internet Protocol addressing scheme to help tackle the issue of shortage of IPv4 addresses.

>Supports up to 2^128 of IP addresses (340 trillion-plus), resolving the issues faced with IPv4

## What is MAC Address ?
>Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard. This network interface is assigned a unique address at the factory it was built at, called a ***MAC (Media Access Control)*** address.

>The MAC address is a **twelve-character hexadecimal number** (a base sixteen numbering system used in computing to represent numbers) split into two's and separated by a colon. These colons are considered separators.

![mac_address](https://user-images.githubusercontent.com/35003220/205228818-77e86395-bf0e-498d-8508-957bfbff7655.png)

## What is Local Area Network (LAN) ?
>A local area network is a computer network that interconnects computers within a limited area such as a residence, school, laboratory, university campus or office building.

## What are Network Topologies ?
>In short, Network topology is a design or look of the network at hand.

>A network topology is the physical and logical arrangement of nodes and connections in a network.

### 1. Star Toplogy
>The main premise of a star topology is that devices are individually connected via a central networking device such as a switch or hub.

>This topology is the most commonly found today because of its reliability and scalability - despite the cost.

>Any information sent to a device in this topology is sent via the central device to which it connects.

>Because more cabling & the purchase of dedicated networking equipment is required for this topology, it is more expensive than any of the other topologies.

>This topology is much more scalable in nature, which means that it is very easy to add more devices as the demand for the network increases.

![star](https://user-images.githubusercontent.com/35003220/205232236-91e00f97-670e-47b1-abfc-b77b2774efc4.png)

### 2. Bus Topology
>This type of connection relies upon a single connection which is known as a backbone cable.

>This type of topology is similar to the leaf off of a tree in the sense that devices (leaves) stem from where the branches are on this cable.

>Because all data destined for each device travels along the same cable, it is very quickly prone to becoming slow and bottlenecked if devices within the topology are simultaneously requesting data.

>This bottleneck also results in very difficult troubleshooting because it quickly becomes difficult to identify which device is experiencing issues with data all travelling along the same route.

![bus](https://user-images.githubusercontent.com/35003220/205232772-b28f0d1a-b38b-400f-86f8-a80123061cbf.png)

### 3. Ring Topology
>The ring topology (also known as token topology) boasts some similarities.

>Devices such as computers are connected directly to each other to form a loop, meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology. 

>A ring topology works by sending data across the loop until it reaches the destined device, using other devices along the loop to forward the data.

>A fault such as cut cable, or broken device will result in the entire networking breaking. 

![ring](https://user-images.githubusercontent.com/35003220/205233394-b1ada41f-b2d6-4cae-83b4-2946485e6d17.png)

## What is Switch ? 
>Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet. 

>These various devices plug into a switch's port. 

>witches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network. 

>Switches can connect a large number of devices by having ports of 4, 8, 16, 24, 32, and 64 for devices to plug into.

> Switches keep track of what device is connected to which port. This way, when they receive a packet, instead of repeating that packet to every port like a hub would do, it just sends it to the intended target, thus reducing network traffic.

![switches](https://user-images.githubusercontent.com/35003220/205233967-f39cfd80-bf6d-4aca-a596-81881a593d4e.png)

## What is Router ?
>It's a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).

>Routing is the label given to the process of data travelling across networks. 

>Routing involves creating a path between networks so that this data can be successfully delivered.

<img width="584" alt="9oRZ5dEIu28zVANhPLh_4pKrOxAr6dFbvslV24RsyuKqC38SqfB6xjuV9zEQf9TxjD4fm2VZIBN8NQvGLTfIeWapeJGwpu6xMpEr8ofRIBA9U7J3mUU201b4J-aogTMApwtoruXX" src="https://user-images.githubusercontent.com/35003220/205234586-bdc0edc4-17f1-4d64-94b5-d85e91efbc8c.png">

## What is Modem ?
>A modem is a device that modulates or demodulates the signal. It maintains a dedicated connection with the ISP to get the internet connection for home or business.

>The modem is placed between the telephone line and the computer system or router.

>It connects the ISP(internet service provider) to the home network directly for the single PC. Or it is connected with the router to connect with multiple devices.

## What is ARP protocol ?
>The ARP protocol or Address Resolution Protocol for short, is the technology that is responsible for allowing devices to identify themselves on a network.

>Simply, the ARP protocol allows a device to associate its MAC address with an IP address on the network.

## How does ARP Work ?
>Each device within a network has a ledger to store information on, which is called a cache. In the context of the ARP protocol, this cache stores the identifiers of other devices on the network.

>In order to map these two identifiers together (IP address and MAC address), the ARP protocol sends two types of messages:

1. ARP Request

2. ARP Reply

>When an ARP request is sent, a message is broadcasted to every other device found on a network by the device, asking whether or not the device's MAC address matches the requested IP address.

>If the device does have the requested IP address, an ARP reply is returned to the initial device to acknowledge this. The initial device will now remember this and store it within its cache (an ARP entry). 

## What is DHCP server & how it works ?
>IP addresses can be assigned either manually, by entering them physically into a device, or automatically and most commonly by using a DHCP (Dynamic Host Configuration Protocol) server.

>When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network.

>The DHCP server then replies back with an IP address the device could use (DHCP Offer).

>The device then sends a reply confirming it wants the offered IP Address (DHCP Request), and then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address (DHCP ACK).

![DHCP](https://user-images.githubusercontent.com/35003220/205316287-8fec7658-6357-4632-91bd-b6f614dd0851.png)


## OSI Model
>The OSI model (or Open Systems Interconnection Model) is an absolute fundamental model used in networking.  This critical model provides a framework dictating how all networked devices will send, receive and interpret data.

![OSI-Table](https://user-images.githubusercontent.com/35003220/205417826-9c4d7d83-aaa6-4a25-bc2c-98b04ff78a7f.png)

    Application   -  All
    Presentation  -  People
    Session       -  Should 
    Transport     -  Try  
    Network       -  New
    Data Link     -  Dominoz
    Physical      -  Pizza
    
### Layer 7 -- Application
>The application layer of the OSI model essentially provides networking options to programs running on a computer.

>It works almost exclusively with applications, providing an interface for them to use in order to transmit data.

>When data is given to the application layer, it is passed down into the presentation layer.

### Layer 6 -- Presentation
>The presentation layer receives data from the application layer. This data tends to be in a format that the application understands, but it's not necessarily in a standardised format that could be understood by the application layer in the receiving computer.

>The presentation layer translates the data into a standardised format, as well as handling any encryption, compression or other transformations to the data. With this complete, the data is passed down to the session layer.

### Layer 5 -- Session
>When the session layer receives the correctly formatted data from the presentation layer, it looks to see if it can set up a connection with the other computer across the network.

>If it can't then it sends back an error and the process goes no further.

>If a session can be established then it's the job of the session layer to maintain it, as well as co-operate with the session layer of the remote computer in order to synchronise communications.

>When the session layer has successfully logged a connection between the host and remote computer the data is passed down to Layer 4: the transport Layer.

### Layer 4 -- Transport
>Its first purpose is to choose the protocol over which the data is to be transmitted.

>The two most common protocols in the transport layer are TCP (Transmission Control Protocol) and UDP (User Datagram Protocol); with TCP the transmission is **connection-based** which means that a connection between the computers is established and maintained for the duration of the request.

>With UDP, the opposite is true; packets of data are essentially thrown at the receiving computer -- if it can't keep up then that's its problem (this is why a video transmission over something like Skype can be pixelated if the connection is bad).

>TCP would usually be chosen for situations where accuracy is favoured over speed (e.g. file transfer, or loading a webpage), and UDP would be used in situations where speed is more important (e.g. video streaming).

>With a protocol selected, the transport layer then divides the transmission up into bite-sized pieces (***over TCP these are called segments, over UDP they're called datagrams***), which makes it easier to transmit the message successfully. 

### Layer 3 -- Network
>The network layer is responsible for locating the destination of your request.

>The network layer is responsible for locating the destination of your request. 

>For example, the Internet is a huge network; when you want to request information from a webpage, it's the network layer that takes the IP address for the page and figures out the best route to take. 

>At this stage we're working with what is referred to as Logical addressing (i.e. IP addresses) which are still software controlled. 

>Logical addresses are used to provide order to networks, categorising them and allowing us to properly sort them.

### Layer 2 -- Data Link
>The data link layer focuses on the physical addressing of the transmission.

> It receives a packet from the network layer (that includes the IP address for the remote computer) and adds in the physical (MAC) address of the receiving endpoint.

>Inside every network enabled computer is a Network Interface Card (NIC) which comes with a unique MAC (Media Access Control) address to identify it.

>MAC addresses are set by the manufacturer and literally burnt into the card; they can't be changed -- although they can be spoofed.

>When information is sent across a network, it's actually the physical address that is used to identify where exactly to send the information.

>Additionally, it's also the job of the data link layer to present the data in a format suitable for transmission.

>The data link layer also serves an important function when it receives data, as it checks the received information to make sure that it hasn't been corrupted during transmission, which could well happen when the data is transmitted by layer 1: the physical layer.

### Layer 1 -- Physical
>The physical layer is right down to the hardware of the computer.

>This is where the electrical pulses that make up data transfer over a network are sent and received.

>It's the job of the physical layer to convert the binary data of the transmission into signals and transmit them across the network, as well as receiving incoming signals and converting them back into binary data.

## What is Encapsulation ?
>Encapsulation is the process of adding additional information when data is traveling in OSI or TCP/IP model.

>The additional information has been added on sender’s side, starting from Application layer to Physical layer.

![image](https://user-images.githubusercontent.com/35003220/205419182-6c67f249-89d5-476f-a628-4376b809d538.jpg)

### How Data Encapsulation works ?
1. There will be no additional information added in the user’s data in the Application layer in TCP/IP model or Application, Presentation, Session layers in OSI model.
2. Then Session layer sends data to Transport layer.
3. In the Transport layer, the data broken up into different pieces. It adds the header in each of the broken data, which contains information like source port, destination port, sequence number, etc. Now, everything combined to a new form.
4. The encapsulated data in Transport layer is called Segments or Datagrams. If the transmission uses TCP, then it is called Segments, or UDP is called Datagrams.
5. Now, the data will travel down and reach Network layer. Here, layer 3 header is added. That contains information like source IP, destination IP, and so on. This information combines into a new form. The encapsulated data in the network layer is called Packets.
6. Now, network layer sends packet to Data Link layer When it enters into data link layer, a new header(Layer 2) is added.
7. Also, a trailer is added. It contains information like source MAC address, destination MAC address, and so on. The trailer is used for error checking. The encapsulated data in the data link layer is called Frames.
8. The physical layer takes frames from Data Link layer. The encapsulated data in the physical layer is called Bits.

That is how encapsulation takes place.

## What is PDU (Protocol Data Unit)?
>The encapsulated data is called by different names when it travels down following layers.

>Those names are called Protocol Data Unit. The following table shows the name of encapsulated data in each layer.

![PDU-283x300](https://user-images.githubusercontent.com/35003220/205419580-b5673bd9-abc0-482a-aef8-e0ef1fbf391f.png)

## What is De-Encapsulation ?
>De-encapsulation is the exact reverse process of encapsulation.

>The additional information added on the sender’s side (during encapsulation) gets removed when it travels on the receiver’s side from the Physical layer to the Application layer.

## TCP/IP Model
>The TCP/IP model is, in many ways, very similar to the OSI model. It's a few years older, and serves as the basis for real-world networking.

>TCP/IP takes its name from the two most important of these: the Transmission Control Protocol (which we touched upon earlier in the OSI model) that controls the flow of data between two endpoints, and the Internet Protocol, which controls how packets are addressed and sent.

>The TCP/IP model consists of four layers: Application, Transport, Internet and Network Interface.

![image-4](https://user-images.githubusercontent.com/35003220/205419868-1a29cf85-d410-422f-84bc-7c99aee639b0.png)

The two models (OSI & TCP/IP) match up something like this:

![image-3](https://user-images.githubusercontent.com/35003220/205419932-6523f88f-d78a-4266-938a-4a27065b7137.png)

>The processes of encapsulation and de-encapsulation work in exactly the same way with the TCP/IP model as they do with the OSI model.

>TCP is a connection-based protocol. In other words, before you send any data via TCP, you must first form a stable connection between the two computers. The process of forming this connection is called the ***three-way handshake***.

### Three Way Handshake 
>When you attempt to make a connection, your computer first sends a special request to the remote server indicating that it wants to initialise a connection.

>This request contains something called a SYN (short for synchronise) bit, which essentially makes first contact in starting the connection process.

>The server will then respond with a packet containing the SYN bit, as well as another "acknowledgement" bit, called ACK. 

>Finally, your computer will send a packet that contains the ACK bit by itself, confirming that the connection has been setup successfully.

>With the three-way handshake successfully completed, data can be reliably transmitted between the two computers.

>Any data that is lost or corrupted on transmission is re-sent, thus leading to a connection which appears to be lossless.

![handshake](https://user-images.githubusercontent.com/35003220/205421263-9b2e56fc-667d-47ee-a0fa-8f9b5aad4d8f.png)









