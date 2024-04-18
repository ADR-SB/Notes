# Network Topologies 

Network topology refers to how various nodes, devices, and connections on your network are physically or logically arranged in relation to each other. 
There are two approaches to network topology:

1. Physical network topology:- physical connections and interconnections between nodes and the network—the wires, cables, and so forth
2. Logical network topology :- little more abstract and strategic, referring to the conceptual understanding of how and why the network is arranged the way it is, and how data moves through it

---
### Point-to-Point
* contain exactly two hosts (computers, switches or routers, servers ) connected back to back using a single piece of cable.
* The receiving end of one host is connected to the sending end of the other and vice-versa. 
* If the hosts are connected point-to-point logically, then they may have multiple intermediate devices. But the end hosts are unaware of the underlying network and see each other as if they are connected directly.

---
## Bus Topology 
* All devices share a single communication line or cable.
* Bus topology may have problems while multiple hosts sending data at the same time.
* Bus topology either uses CSMA/CD technology or recognizes one host as Bus Master to solve the issue.
* failure of a device does not affect the other devices.
* Both ends of the shared channel have a line terminator. The data is sent in only one direction and as soon as it reaches the extreme end, the terminator removes the data from the line. 

__Point of failure:__
* failure of the shared communication line can make all other devices stop functioning.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Star Topology 
* All hosts in Star topology are connected to a central device (hub) 
* The hub uses a point-topoint connection. (ie; there exists a point to point connection between hosts and hub).
* The hub device can be any of the following: 
 
	* Layer-1 device such as hub or repeater 
	* Layer-2 device such as switch or bridge 
	* Layer-3 device such as router or gateway 
   
* Every communication between hosts takes place through only the hub. 
* Star topology is not expensive.
* only one cable is required to connect one more host and configuration is simple. 
	
__Point of failure:__
* hub acts as a single point of failure (If the hub fails, connectivity of all hosts to all other hosts fails).

---
### Ring Topology 
* each host machine connects to exactly two other machines, creating a circular network structure. 
* When one host tries to communicate or send message to a host which is not adjacent to it, the data travels through all intermediate hosts. 
* To connect one more host in the existing structure, the administrator may need only one more extra cable. 
* There are methods which employ one more backup ring. 

__Point of failure:__
* every connection in the ring is a point of failure. ( Failure of any host results in failure of the whole ring).

---
### Mesh Topology 
* host is connected to one or multiple hosts. 
* pointto-point connection with every other host or may also have hosts which are in point-to-point connection to few hosts only. 
* Hosts in Mesh topology also work as relays for other hosts which do not have direct point-to-point links. 
* Mesh technology comes into two types: 
 
	* Full Mesh: All hosts have a point-to-point connection to every other host in the network. Thus for every new host n(n-1)/2 connections are required. It provides the most reliable network structure among all network topologies. 
	* Partially Mesh: Not all hosts have point-to-point connection to every other host. Hosts connect to each other in some arbitrary fashion. This topology exists where we need to provide reliability to some hosts out of all. 

---
### Tree Topology (Hierarchical Topology) 
* most common form of network topology in use presently. 
* This topology imitates as extended Star topology and inherits properties of bus topology. 
* divides the network in to multiple levels/layers of the network. 
* Mainly in LANs, a network is bifurcated into three types of network devices. 
	1. The lowermost is an access-layer where computers are attached. 
	2. The middle layer is known as the distribution layer, which works as a mediator between upper layer and lower layer. 
	3.The highest layer is known as the core layer, and is the central point of the network, i.e. root of the tree from which all nodes fork. 
* All neighboring hosts have point-to-point connection between them.  

__Point of failure:__
* Similar to the Bus topology, if the root goes down, then the entire network suffers even. Though it is not the single point of failure. 
* Every connection serves as a point of failure, failing which divides the network into unreachable segments.

---
### Daisy Chain 
* connects all the hosts in a linear fashion. 
* Similar to Ring topology, all hosts are connected to two hosts only, except the end hosts. 
* if the end hosts in daisy chain are connected then it represents Ring topology. 
 
	* Each link in daisy chain topology represents single point of failure.  
	* Every intermediate host works as relay for its immediate hosts. 

__Point of failure:__
* Every link failure splits the network into two segments.

---
### Hybrid Topology 
* contains more than one topology. 
* inherits merits and demerits of all the incorporating topologies. 
* The combining topologies may contain attributes of Star, Ring, Bus, and Daisy-chain topologies. 
* Internet is the best example of largest Hybrid topology.

---

