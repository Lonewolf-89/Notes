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











