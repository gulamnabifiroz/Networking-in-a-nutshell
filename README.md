# Networking-in-a-nutshell
Computer networking is the practice of connecting multiple devices—like computers, phones, and servers—so they can share data and resources. Computer network is a collection of interconnected devices that communicate with each other to exchange data and resources. It enables efficient communication and supports services like email, file sharing, and internet access.

##  Flow of Networks
* Nodes are physical devices such as computers, mobiles, or printers.
* Routers and switches control the flow of information.
* Transmission media carry data from one device to another.
* Wired media includes Ethernet and optical fiber cables.

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/e54ba121-3351-4cab-be1a-22f2f3681003" />

## Types of Computer Network Architecture

<img width="1676" height="788" alt="image" src="https://github.com/user-attachments/assets/7bbbed70-847d-4fba-9e90-515646db7f60" />

### Client-Server Architecture: 
Represents a type of computer network architecture in which nodes function as servers or clients, where the server manages client behavior, known as Client-Server Architecture.
### Peer-to-Peer Architecture:
Operates without any central server, allowing each device to act as either a client or a server, known as P2P (Peer-to-Peer) Architecture.

### Network Devices
These are physical devices that connect computers, printers and other electronic equipment to a network and enable data sharing, transferring and managing.

## 1. Router
* Functions as a networking device that connects multiple networks and directs data between them.
* Connects local networks to the internet
* Determines the best path for data packets
* Uses IP addresses to forward data correctly

## 2. Switch
* Connects devices within the same network and manages internal data communication.
* Connects computers, printers, and servers
* Sends data only to the intended device
* Improves network efficiency and performance

## 3. Hub
* Acts as a basic device that connects multiple devices within a network.
* Broadcasts data to all connected devices
* Does not filter or manage traffic
* Less secure and less efficient than a switch

## 4. Bridge
* Connects two network segments and filters traffic between them.
* Reduces unnecessary data transmission
* Improves network performance
* Works using MAC addresses

## 5. Gateway
* Connects two different networks that use different protocols.
* Translates data between different systems
* Enables communication between dissimilar networks
* Commonly used to connect private networks to external networks

## 6. Access Point (AP)
* Provides wireless connectivity to devices in a network.
* Extends a wired network into Wi-Fi
* Allows mobile devices to connect wirelessly
* Improves network coverage area

## 7. Modem
* Converts digital data into signals suitable for transmission and vice versa.
* Connects a home or office network to the ISP
* Converts digital signals to analog and back
* Enables internet access

## 8. Firewall
* Security device that monitors and controls network traffic.
* Blocks unauthorized access
* Filters incoming and outgoing data
* Protects networks from cyber threats

### OSI Model
The OSI Model is a conceptual framework created by the International Organization for Standardization (ISO) to describe how data is transmitted across a network using a structured seven-layer architecture.
<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/bc292c87-6007-4345-b327-e840476a82ca" />

## 1. Physical Layer
* Transmits raw bit streams over a physical medium.
* Defines electrical, mechanical, and physical specifications for devices and cables.
* Deals with bit synchronization, line configuration, and transmission mode (simplex, half-duplex, full-duplex).
* Key hardware includes cables, hubs, repeaters, and network interface cards (NICs).

## 2. Data Link Layer
* Provides node-to-node data transfer and detects/corrects errors that occur in the Physical layer.
* Encapsulates packets into frames.
* Divided into two sublayers: Media Access Control (MAC) and Logical Link Control (LLC).
* Manages physical addressing (MAC addresses) and flow control.

## 3. Network Layer
* Responsible for routing data packets from the source host to the destination host across different networks.
* Handles logical addressing (IP addresses).
* Determines the best physical path for the data to travel using routing algorithms.
* Key devices include routers and layer-3 switches.

## 4. Transport Layer
* Ensures reliable, end-to-end data transfer and segment delivery between hosts.
* Provides flow control, error checking, and data segmentation/reassembly.
* Uses protocols like TCP (Transmission Control Protocol) for reliable delivery and UDP (User Datagram Protocol) for fast, connectionless delivery.
* Manages port addressing to ensure data reaches the correct application.

## 5. Session Layer
* Establishes, manages, maintains, and terminates communication sessions between local and remote applications.
* Handles authentication and authorization to secure the connection.
* Inserts checkpoints into data transfers so that transmission can resume from the last checkpoint in case of a network failure.

## 6. Presentation Layer
* Translates data between the application layer format and the network format.
* Responsible for data formatting, syntax conversion, and data compatibility.
* Handles data compression to reduce bandwidth consumption and data encryption/decryption for security.

## 7. Application Layer
* Interacts directly with the user software or application to provide network services.
* Serves as the window for users and application processes to access network services.
* Utilizes high-level protocols such as HTTP, HTTPS, FTP, SMTP, and DNS.

## Network Topologies
Defines the geometric arrangement of various links and nodes in a network.
* **Mesh Topology:** Every device is connected to every other device; highly redundant, reliable, but expensive.
* **Star Topology:** All devices connect to a central hub or switch; easy to troubleshoot but creates a single point of failure.
* **Bus Topology:** All devices share a single backbone cable; simple for small networks but fails entirely if the backbone breaks.
* **Ring Topology:** Devices are connected in a closed loop; data travels in one direction, preventing data collisions but risking complete failure if one node drops.

## IPV4 vs IPV6
* **Address Space:** IPv4 uses a 32-bit address allowing for roughly 4.3 billion unique addresses, whereas IPv6 uses a 128-bit address, providing an almost infinite number of unique addresses ($3.4 \times 10^{38}$).
* **Address Format:** IPv4 addresses are written in dotted-decimal notation (e.g., `192.168.1.1`), while IPv6 addresses use hexadecimal notation separated by colons (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
* **Configuration:** IPv4 requires manual setup or DHCP configuration, whereas IPv6 supports stateless address autoconfiguration (SLAAC), allowing devices to generate their own addresses automatically.
* **Security:** Internet Protocol Security (IPsec) is optional in IPv4 but is built into the core blueprint of IPv6.
* **Header Complexity:** IPv4 has a variable header length (20 to 60 bytes) with 12 fields, while IPv6 features a simplified, fixed header length (40 bytes) with only 8 fields to improve routing efficiency.
* **Packet Fragmentation:** In IPv4, packet fragmentation can be done by both the sending host and intermediate routers. In IPv6, fragmentation is handled strictly by the sending host, reducing network bottlenecking.

