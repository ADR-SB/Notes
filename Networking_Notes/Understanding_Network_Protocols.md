# Understanding Network Protocols  
* A network protocol is an established set of rules that determine how data is transmitted between different devices in the same network. Essentially, it allows connected devices to communicate with each other, regardless of any differences in their internal processes, structure or design.
* Network protocols are the reason you can easily communicate with people all over the world.
* Similar to the way that speaking the same language simplifies communication between two people, network protocols make it possible for devices to interact with each other because of predetermined rules built into devices’ software and hardware.

---
## OSI Model
* The open systems interconnection (OSI) model is a conceptual model created by the International Organization for Standardization.
* it enables diverse communication systems to communicate using standard protocols.
* It’s based on the concept of splitting up a communication system into seven abstract layers, each one stacked upon the last.

### Why does the OSI model matter? 
* Although the modern Internet doesn’t strictly follow the OSI Model (it more closely follows the simpler Internet protocol suite), the OSI Model is still very useful for troubleshooting network problems.
* the OSI Model can help to break down problems and isolate the source of the trouble.
* If the problem can be narrowed down to one specific layer of the model, a lot of unnecessary work can be avoided.

### The seven abstraction layers of the OSI model can be defined as follows, from top to bottom:
#### 7. Application Layer 
* only layer that directly interacts with data from the user. 
* Software applications like web browsers and email clients rely on the application layer to initiate communications.
  * client software applications are not part of the application layer; rather the application layer is responsible for the protocols and data manipulation that the software relies on to present meaningful data to the user. 
* Application layer protocols include HTTP as well as SMTP (Simple Mail Transfer Protocol is one of the protocols that enables email communications).

#### 6. Presentation Layer 
* primarily responsible for preparing data so that it can be used by the application layer; in other words, layer 6 makes the data presentable for applications to consume.
* The presentation layer is responsible for translation, encryption, and compression of data. 
* Two communicating devices communicating may be using different encoding methods, so layer 6 is responsible for translating incoming data into a syntax that the application layer of the receiving device can understand. 
* If the devices are communicating over an encrypted connection, layer 6 is responsible for adding the encryption on the sender’s end as well as decoding the encryption on the receiver's end so that it can present the application layer with unencrypted, readable data. 
* Finally, the presentation layer is also responsible for compressing data it receives from the application layer before delivering it to layer 5. This helps improve the speed and efficiency of communication by minimizing the amount of data that will be transferred.

#### 5. Session Layer 
* This is the layer responsible for opening and closing communication between the two devices.
* The time between when the communication is opened and closed is known as the session.
* The session layer ensures that the session stays open long enough to transfer all the data being exchanged, and then promptly closes the session in order to avoid wasting resources. 

__The session layer also synchronizes data transfer with checkpoints.__ For example, if a 100-megabyte file is being transferred, the session layer could set a checkpoint every 5 megabytes. In the case of a disconnect or a crash after 52 megabytes have been transferred, the session could be resumed from the last checkpoint, meaning only 50 more megabytes of data need to be transferred. Without the checkpoints, the entire transfer would have to begin again from scratch. 
 
#### 4. Transport Layer 
* Layer 4 is responsible for end-to-end communication between the two devices. 
* This includes taking data from the session layer and breaking it up into chunks called segments before sending it to layer 3. The transport layer on the receiving device is responsible for reassembling the segments into data the session layer can consume. 
* The transport layer is also responsible for flow control and error control. 
* Flow control determines an optimal speed of transmission to ensure that a sender with a fast connection doesn’t overwhelm a receiver with a slow connection. 
* The transport layer performs error control on the receiving end by ensuring that the data received is complete, and requesting a retransmission if it isn’t. 
 
#### 3. Network Layer 
* The network layer is responsible for facilitating data transfer between two different networks. 
* If the two devices communicating are on the same network, then the network layer is unnecessary.
* The network layer breaks up segments from the transport layer into smaller units, called packets, on the sender’s device, and reassembles these packets on the receiving device. 
* The network layer also finds the best physical path for the data to reach its destination; this is known as routing. 
 
#### 2. Data-Link Layer 
* The data link layer is very similar to the network layer
* data link layer facilitates data transfer between two devices on the SAME network. 
* The data link layer takes packets from the network layer and breaks them into smaller pieces called frames. 
* Like the network layer, the data link layer is also responsible for flow control and error control in intra-network communication (The transport layer only does flow control and error control for inter-network communications). 
 
#### 1. Physical Layer 
* This layer includes the physical equipment involved in the data transfer, such as the cables and switches. 
* This is also the layer where the data gets converted into a bit stream, ( string of 1s and 0s. )
* The physical layer of both devices must also agree on a signal convention so that the 1s can be distinguished from the 0s on both devices. 

