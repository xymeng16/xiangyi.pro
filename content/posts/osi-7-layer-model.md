---
title: "OSI 7-Layer Model"
date: 2020-09-10T10:29:19Z
draft: false
---

The Open System Interconnection (OSI) model (defined in [ISO 7498-1](https://www.iso.org/standard/20269.html)), which is a reference tool for understanding data communications between two networked systems, divides the communication processes into 7 layers:
1. Physical layer
2. Data link layer
3. Network layer
4. Transport layer
5. Session layer
6. Presentation layer
7. Application layer  

Those layers break up the networks into manageable pioeces, which provides a common language to explain components and their functionalities. Here this article will give an overview of the 7 layers top-to-down.  

## Layer 7: The Application Layer
OSI Model, Layer 7, supports application and end-user processes. Communication partners are identified, quality of service is identified, user authentication and privacy are considered, and any constraints on data syntax are identified. Everything at this layer is application-specific. This layer provides application services for file transfers, e-mail, and other network software services. Telnet and FTP are applications that exist entirely in the application level. Tiered application architectures are part of this layer.

## Layer 6: The Presentation Layer
This layer provides independence from differences in data representation (e.g., encryption) by translating from application to network format, and vice versa. The presentation layer works to transform data into the form that the application layer can accept. This layer formats and encrypts data to be sent across a network, providing freedom from compatibility problems. It is sometimes called the syntax layer.

## Layer 5: The Session Layer
This layer establishes, manages and terminates connections between applications. The session layer sets up, coordinates, and terminates conversations, exchanges, and dialogues between the applications at each end. It deals with session and connection coordination.

## Layer 4: The Transport Layer
Layer 4 provides transparent transfer of data between end systems, or hosts, and is responsible for end-to-end error recovery and flow control. It ensures reliable data transfer.

## Layer 3: The Network Layer
The network layer provides switching and routing technologies, creating logical paths, known as virtual circuits, for transmitting data from node to node. Routing and forwarding are functions of this layer, as well as addressing, internetworking, error handling, congestion control and packet sequencing.

## Layer 2: The Data Link Layer
This layer provides node-to-node data transfer (between two directly connected nodes), and also handles error correction from the physical layer. Here data packets are encoded and decoded into bits. In this layer, data packets have a unique name: frames. And it's divided into 2 sub-layers: the Media Control Access (MAC) layer and the Logical Link Control (LLC) layer. The MAC sub layer controls how a computer on the network gains access to the data and permission to transmit it. The LLC layer controls frame synchronization, flow control and error checking.

## Layer 1: The Physical Layer
The physical layer defines specifications of connector and interface, as well as the medium (cable) requirements. Electrical, mechanical, functional, and procedural specifications are provided for sending a bit stream on a computer network.  
