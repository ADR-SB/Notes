# Understanding Network Hardware  
 
Networking hardware, also known as network equipment or computer networking devices, are electronic devices which are required for communication and interaction between devices on a computer network. Specifically, they mediate data transmission in a computer network.  

---
## Repeater 
  
* network devices operating at the physical layer of the OSI model 
* it amplify or regenerate an incoming signal before retransmitting it. 
* They are incorporated in networks to expand its coverage area. 
* also known as signal boosters. 
 
### Why are Repeaters needed? 

* When an electrical signal is transmitted via a channel, it gets attenuated depending upon the nature of the channel or the technology. This poses a limitation upon the length of the LAN or coverage area of cellular networks. 
* This problem is alleviated by installing repeaters at certain intervals. 
* Repeaters amplify the attenuated signal and then retransmits it. 
* Digital repeaters can even reconstruct signals distorted by transmission loss.So, repeaters are popularly incorporated to connect between two LANs thus forming a large single LAN. This is shown in the following diagram: 
 
 ### Types of Repeaters 
According to the types of signals that they regenerate, repeaters can be classified into two categories: 
* Analog Repeaters − They can only amplify the analog signal. Digital Repeaters − They can reconstruct a distorted signal. 
 
According to the types of networks that they connect, repeaters can be categorized into two types: 
* Wired Repeaters − They are used in wired LANs. 
* Wireless Repeaters − They are used in wireless LANs and cellular networks. 
 
According to the domain of LANs they connect, repeaters can be divided into two categories: 
* Local Repeaters − They connect LAN segments separated by small distances. 
* Remote Repeaters − They connect LANs that are far from each other. 

### Advantages of Repeaters 
* simple to install and can easily extend the length or the coverage area of networks. 
* They are cost effective. 
* Repeaters don’t require any processing overhead. The only time they need to be investigated is in case of degradation of performance. 
* They can connect signals using different types of cables. 
 
### Disadvantages of Repeaters 
* cannot connect dissimilar networks. 
* They cannot differentiate between actual signal and noise. 
* They cannot reduce network traffic or congestion. 
* Most networks have limitations upon the number of repeaters that can be deployed. 
 
---
## Hubs 
  
*  physical layer networking device 
* used to connect multiple devices in a network. 
* They are generally used to connect computers in a LAN. 
* A hub has many ports in it. A computer which intends to be connected to the network is plugged into one of these ports. When a data frame arrives at a port, it is broadcast to every other port, without considering whether it is destined for a particular destination or not. 
 
---
## Switches 
  
* data link layer networking device 
* connects devices in a network and uses __packet__ __switching__ to send and receive data over the network. 
* Like a hub, a switch also has many ports, to which computers are plugged in. However, when a data frame arrives at any port of a network switch, it examines the destination address and sends the frame to the corresponding device(s). Thus, it supports both unicast and multicast communications. 
 
 
### Features of Switches 
* A switch operates in the layer 2, i.e. data link layer of the OSI model. 
* It is an intelligent network device that can be conceived as a multiport network bridge. 
* It uses MAC addresses (addresses of medium access control sublayer) to send data packets to selected destination ports. 
* It uses packet switching technique to receive and forward data packets from the source to the destination device. 
* It supports unicast (one-to-one), multicast (one-to-many) and broadcast (one-to-all) communications. 
* Transmission mode is full duplex, i.e. communication in the channel occurs in both the directions at the same time. Due to this, collisions do not occur. 
* Switches are active devices, equipped with network software and network management capabilities. 
* Switches can perform some error checking before forwarding data to the destined port. 
* The number of ports is higher – 24/48. 
 
### Types of Switches 
* can be broadly categorized into 4 types: 
	1. Unmanaged Switch: 
		* inexpensive switches commonly used in home networks and small businesses. 
		* can be set up by simply plugging in to the network, after which they instantly start operating. 
		* plug and play method used to add more devices. 
		* do not require to be configured or monitored. 
 
	2. Managed Switch: 
		* costly switches that are used in organizations with large and complex networks
		* they can be customized to augment the functionalities of a standard switch. 
		* The augmented features may be QoS (Quality of Service) like higher security levels, better precision control and complete network management. 
		* Despite their cost, they are preferred in growing organizations due to their scalability and flexibility. Simple Network Management Protocol (SNMP) is used for configuring managed switches. 
 
	3. LAN Switch: 
		* connect devices in the internal LAN of an organization. 
		* also referred to as Ethernet switches or data switches. 
		* helpful in reducing network congestion or bottlenecks. 
		* They allocate bandwidth in a manner so that there is no overlapping of data packets in a network. 
 
	4. PoE Switch: 
		* Power over Ethernet (PoE) switches are used in PoE Gigabit Ethernets. 
		* PoE technology combines data and power transmission over the same cable 
		* devices connected to it can receive both electricity as well as data over the same line. 
		* PoE switches offer greater flexibility and simplifies the cabling connections. 
 
### Differences between Hub and Switch 
| Hub | Switch |
|:------|:----------| 
| operate in the physical layer of the OSI model. | operate in the data link layer of the OSI model. |
| non-intelligent network device that sends messages to all ports. | intelligent network device that sends messages to selected destination ports. |
| primarily broadcasts messages. | supports unicast, multicast and broadcast. | 
| Transmission mode is half duplex. |	Transmission mode is full duplex. | 
| Collisions may occur during setup of transmission when more than one computer places data simultaneously in the corresponding ports. |	Collisions do not occur since the communication is full duplex. |
| They are passive devices, they don’t have any software associated with it. |	They are active devices, equipped with network software. |
| They generally have fewer ports of 4/12. |	The number of ports is higher – 24/48. | 
 
--- 
## Routers 
  
* used to connect two or more subnets that cannot be similar.
* They operate at the OSI model’s network layer
* These devices support connectedness between two LANs or two WANs over the large geographical range.
* The routers evaluate the best route from a sender to a receiver.
* For this, they perform in a routing protocol to create the network topology, and the data thus gathered is used to evaluate routes.
* Routers are generally a mixture of hardware and software.
* The hardware includes physical interfaces to various networks, while the software consists of an operating system and routing protocol.
* They use both logical and physical transmitting to link two or more logically separate networks. The figure shows three types of LANs connected by a single router. 
* For this, each network to be connected is allocated a logical address, and then these logical segments are combined by the router in a large network. They use the store and forward technique to transmit the message, i.e., receive messages, check their destination and send the needed LAN message. 
 
### Types of Routers 
1. Central Router: Central router is a router that acts as the backbone of a network. It connects many LANs. 
2. Local Router: The local router has limitations to operate within the limits of its LAN driver’s cable length limitations. 
3. Remote Router: A remote router uses modems or remote connections to connect the LANs beyond its device driver limitations. 
4. Internal Router: Internal router is a part of the network file server, and it routes the data accordingly. External Router: The external router is located in a workstation on the network. 
5. Peripheral Router: The peripheral router links single LANs to a central router or sometimes to another peripheral router. 
 
### Features of Routers 
* Routers are multiport tools with huge speed backbones. 
* It is used to provide penetrating and encapsulation like bridges. 
* Routers continuously monitor the network’s condition to adapt to changes in the network’s condition dynamically. 
* They generally support some method of redundancy so that they are less prone to catastrophic failure. 

---
## GATEWAY 
  
* A device that can bridge several network structures is called a gateway. Thus gateways can link two dissimilar LANs.
* The major difference between gateways and routers is that routers operate at the OSI model’s network layer. In contrast, gateways operate from the lowest to the topmost layer, i.e., the application layer to the OSI model’s network layer. 
* Gateways and routers are used correspondingly. It can change data packets from one protocol structure to another before forwarding them to connect two different networks. Hence it incorporates a protocol conversion function at the application layer. 
* A gateway is a connecting device that can relate to multiple networks. They perform at the application layer of the OSI model. They manage messages, locations, and protocol conversion to deliver a packet to its terminal between two connections. 
* gateways are slow because they need to perform intensive conversions. 
 
### Characteristics of Gateways 
* It can support complete protocol transformation from one proprietary computer network technology to other technology. It means ethernet to token ring or FDDI or some different model or protocol instead of encapsulation. 
* It needs higher layers of the OSI model, possible by layer 7, the application layer. IBM SNA, DECnet, Internet TCP/IP and other protocols can be transformed from connection to connection. 
	Unlike bridges and routers, gateways work casually due to protocol conversion. Therefore, they can generate bottlenecks of the blockage during the time of peak operation. 
 
### Advantages of Gateways 
* It can connect the devices of two several networks having a different design. 
* It is an intelligent tool with filtering capabilities. 
* It has control over both collisions and the advertisement area. 
* It needs a full-duplex mode of connection. 
* It can make data translation and protocol conversion of the data packet according to the destination network's requirements. 
* It is used to encapsulate and decapsulate the data packets. 
* It has enhanced security over any other network-related device. 
 
--- 
## NIC Card 
  
* A NIC (Network Interface Card) provides the hardware interface between a computer and a network. 
* almost all new computer motherboards have in-built NIC (Network Interface Card). 
* Some NIC (Network Interface Card) cards are meant for wired networks while others are for wireless networks.
* Most widely used wired LAN Technology is Ethernet. Ethernet based NIC (Network Interface Card) cards are available in every local electronic hardware shops. Normal speed rating of Ethernet based wired NIC (Network Interface Card) available these days are 10/100/1000 Mbps (Megabits per second). 
* Every computer participating in the network must have at least one NIC. Computers can have more than one NIC card also, if required. 
 
Every NIC (Network Interface Card) has a 48-bit globally unique identifier called MAC Address (Media Access Control Address) burned into its ROM chip. This MAC address is used to deliver Ethernet Frames to a computer. 
The NIC driver software passes the data between the Operating System and the NIC. Latest Operating Systems include different NIC driver software for almost all major NIC vendors. If your NIC card is not detected or not working, you must find a suitable NIC driver software from the NIC vendor's website and install it on the computer. 
 
 
* MAC address is the physical address, which uniquely identifies each device on a given network. To make communication between two networked devices, we need two addresses: IP address and MAC address. It is assigned to the NIC (Network Interface card) of each device that can be connected to the internet. 
* It stands for Media Access Control, and also known as Physical address, hardware address, or BIA (Burned In Address). 
* It is globally unique; it means two devices cannot have the same MAC address. It is represented in a hexadecimal format on each device, such as 00:0a:95:9d:67:16. 
 
* It is 12-digit, and 48 bits long, out of which the first 24 bits are used for OUI(Organization Unique Identifier), and 24 bits are for NIC/vendor-specific. 
* It is provided by the device's vendor at the time of manufacturing and embedded in its NIC, which ideally cannot be changed. 

---
