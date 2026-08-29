# OSI Model Layers & Functions
OSI stands for open systems interconnection is helpful to understand how data travels through internet. It  has seven layers they are:- 
- Application Layer
- Presentation Layer
- Session Layer
- Transport Layer
- Network Layer
- Data link Layer
- Physical Layer
  
 each layer performs specific function

## Function of each Layer

  ### 7. Application Layer:-
    it is the layer where user interacts with network services.
    ###### Example:- A user searching for google in the browser on the search box this happens in the application layer. 
  ### 6. Presentation Layer:-
    Presentation layer performs how data is being presented or formatted so another computer can understand it. 
    ###### Example:- Data formatting, Compression, Encryption
  ### 5. Session Layer:- 
    In session layer creates a session between the two devices. The session layer Establishes, manages and terminates communication sessions between 2 devices.
  ### 4. Transport Layer:- 
    Transport layer does provide end-to-end communication between devices. It divides the data into segments and ensures reliable or fast deliver using TCP and UDP.
  ### 3. Network Layer:- 
    The Network layer provides logical address and routes the data packets between different networks using routers
  ### 2. Data Link Layer:-
    Data link layer uses the MAC address to communicate within the local network. It is responsible for switching and framing.
  ### 1. Physical Layer:- 
    The Physical layer is responsible for transmitting the raw bits (0s and 1s) through a physical media such as cables or fiber optics.
# TCP/IP Protocol suite
The TCP/IP Protocol Suite (Transmission Control Protocol/Internet Protocol) is a collection of communication protocols that enables computers and devices to communicate over the internet and private networks. It has four layers they are:-
- Application Layer
- Transport Layer
- Internet Layer
- Network access Layer
### 1. Application Layer
- Provides network services directly to user applications.
- Combines the functions of the OSI Application, Presentation, and Session layers.
  
###### Common protocols:
- HTTP/HTTPS –> Web browsing
- FTP –> File transfer
- SMTP –> Email sending
- POP3/IMAP –> Email retrieval
- DNS –> Domain name resolution
- Telnet/SSH –> Remote login
### 2. Transport layer
- Ensures end-to-end communication between devices.
- Responsible for data segmentation, error checking, flow control, and reliability.
###### Protocols:
1. TCP (Transmission Control Protocol):
Connection-oriented
Reliable data delivery
Error detection and retransmission
Used by HTTP, FTP, SMTP
2. UDP (User Datagram Protocol):
Connectionless
Faster but less reliable
Used for streaming, online gaming, VoIP, DNS
### 3. Internet layer
- Responsible for logical addressing and routing packets between networks.
###### Protocols:
- IP (Internet Protocol) –> Provides logical addressing (IPv4, IPv6)
- ICMP –> Error reporting and diagnostics (e.g., ping)
- ARP –> Maps IP addresses to MAC addresses (IPv4)
- IGMP –> Manages multicast groups
### 4. Network access layer
- Handles physical transmission of data over the network.
- Responsible for framing, MAC addressing, and error detection on the local network.
###### Technologies:
- Ethernet
- Wi-Fi (IEEE 802.11)
- PPP
- Frame Relay
# DNS
DNS stands for Domain Name System. It is used to convert the domain names into the IP addresses. Computers uses IP addresses to communicate but humans prefer Names to remember easily. 
###### Example:
You type: www.google.com -> DNS finds: 142.250.10.5
-  Your computer → Google server
###### How DNS works:
- User: Suppose user types for google in search box.
- Web browser: Web browser takes the request of user
- DNS resolver: The request goes to a DNS resolver, commonly provided by your ISP or a public DNS service.
- Root server: If necessary, the resolver asks a root DNS server: "Who handles .com?"
- TLD server: The .com server tells the resolver which authoritative DNS server handles example.com.
- Authoritative DNS server: It provides the actual IP address.
  ###### example:  example.com → 93.184.216.34
- Browser connects to the server: Now the browser can communicate with the web server.
- 
# HTTP - Hypertext Transfer Protocol
HTTP is an application layer protocol used for communication between a client and a web server. Port number is 80. HTTP data is not encrypted in transit.
##### HTTP Request:- An HTTP REQUEST is a message sent from the client to the server asking for resources.
##### HTTP Response:- An HTTP Response is the server's reply to the client
##### HTTP Methods:- 
When a browser sends an HTTP request, it tells the server what action it wants to perform. This action is called an HTTP Method
| Method | Purpose | 
|---|---|
| `GET` | Retrieve data |
| `POST` | Send new data | 
| `PUT` | update existing data |
| `DELETE` | Delete data |
##### HTTP Status codes:-
When a server responds to an HTTP request, it also sends a status code. the status code tells the client whether the request was successful or if there was a problem
| Status code | Meaning | 
|---|---|
| `100` | Continue |
| `200 ok` | request was successful | 
| `301` | Moved permanently |
| `302` | Temporary redirect |
| `403` | Forbidden |
| `404` | Not found |
| `500` | Internal server error |
# HTTPS - Hypertext Transfer Protocol Secure
- HTTPs is an application layer protocol used for communication between a client and a web server. Port number is 443. HTTPs data is encrypted in transit.
- The browser verifies the server's digital certificate.
- After the TLS handshake establishes the cryptographic session, HTTP data is transmitted through the encrypted TLS connection.
# IP Address
Ip address is a logical address and unique number having for each device. It helps identify the devices and communicate with each other.
   #### IPV4 address
- IPV4 (Internet protocol version 4) is the fourth version of IP. It uses 32bits of address to identify the device.
- It is divided into 4 octets, each containing 8 bits.
   ###### Example 
192.168.1.10
   #### Private Ip Address
private address are used within the local networks like College, Office, Home, etc..,
Ranges are
- 10.0.0.0  -  10.255.255.255
- 172.16.0.0  -  172.31.255.255
- 192.168.0.0  -  192.168.255.255

Common Examples of IP address:-
Laptop  → 192.168.1.10
Phone   → 192.168.1.11
TV      → 192.168.1.12
  #### Public IP Address
A public IP is used for communication across the Internet.
  ###### Phone (192.168.1.3) -> Lap (192.168.1.2) -> Router -> Public IP(49.205.100.25) -> Internet
# Subnetting
Subnet is the practice of diving thee large network into two or more networks is called subnetting.
###### example:
192.168.1.0/24
#### Subnet Mask
- A subnet mask tells us which portion of an IPv4 address represents the network and which portion represents the host.
- In above example 24 Networks bits and 8 Host bits
- /24 has:32 - 24 = 8 host bits
  ###### Therefore:
2⁸ = 256 addresses
- But two addresses are traditionally reserved:
- Network address
- Broadcast address
- So usable host addresses:256 - 2 = 254
###### Therefore:
- Network:   192.168.1.0
- Usable:    192.168.1.1 – 192.168.1.254
- Broadcast: 192.168.1.255
# NAT — Network Address Translation
- NAT allows private IP addresses to communicate with the Internet by translating addresses at a router/firewall.
- The private address(192.168.1.10) is translated to a public address when traffic goes out to the Internet.
Laptop(192.168.1.10) -> Router -> Public IP -> Internet
#### Types of NAT
1. Static NAT
   Useful when an internal server needs a consistent public address.
2. Dynamic NAT
   Private addresses are mapped to addresses from a pool of public addresses.
3.PAT — Port Address Translation
Many private devices share one public IP, with different source ports allowing the router to distinguish connections.   
  
   





















    
