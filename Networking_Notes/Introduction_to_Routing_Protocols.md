# Routing Protocols 
 
## What is routing? 
  
* Network routing is the process of selecting a path across one or more networks.
* The principles of routing can apply to any type of network, from telephone networks to public transportation.
* In packet switching networks, such as the Internet, routing selects the paths for Internet Protocol (IP) packets to travel from their origin to their destination.
* These Internet routing decisions are made by specialized pieces of network hardware called routers. 

 
##  How does routing work? 
  
* Routers refer to internal routing tables to make decisions about how to route packets along network paths.
* A routing table records the paths that packets should take to reach every destination that the router is responsible for.
* Routers work in the following way: when a router receives a packet, it reads the headers* of the packet to see its intended destination. It then determines where to route the packet based on information in its routing tables. 
* Routers do this millions of times a second with millions of packets.
* As a packet travels to its destination, it may be routed several times by different routers. 
* Routing tables can either be static or dynamic.
  * Static routing tables do not change. A network administrator manually sets up static routing tables. This essentially sets in stone the routes data packets take across the network, unless the administrator manually updates the tables. 
  * Dynamic routing tables update automatically. Dynamic routers use various routing protocols to determine the shortest and fastest paths. They also make this determination based on how long it takes packets to reach their destination.
* Dynamic routing requires more computing power.
* which is why smaller networks may rely on static routing. But for medium-sized and large networks, dynamic routing is much more efficient. 
 
##  What are the main routing protocols? 
  
* A routing protocol is a protocol used for identifying or announcing network paths. 
 
### The following protocols help data packets find their way across the Internet: 
* IP: The Internet Protocol (IP) specifies the origin and destination for each data packet. Routers inspect each packet's IP header to identify where to send them. 
* BGP: The Border Gateway Protocol (BGP) routing protocol is used to announce which networks control which IP addresses, and which networks connect to each other. (The large networks that make these BGP announcements are called autonomous systems.) BGP is a dynamic routing protocol. 
 
### The below protocols route packets within an AS: 
* OSPF: The Open Shortest Path First (OSPF) protocol is commonly used by network routers to dynamically identify the fastest and shortest available routes for sending packets to their destination. 
* RIP: The Routing Information Protocol (RIP) uses "hop count" to find the shortest path from one network to another, where "hop count" means number of routers a packet must pass through on the way. (When a packet goes from one network to another, this is known as a "hop.") 
 
Other interior routing protocols include EIGRP (the Enhanced Interior Gateway Routing Protocol, mainly for use with Cisco routers) and IS-IS (Intermediate System to Intermediate System). 
