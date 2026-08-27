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
HTTP is an application layer protocol used for communication between a client and a web server.
##### HTTP Request:- An HTTP REQUEST is a message sent from the client to the server asking for resources.
##### HTTP Response:- An HTTP Response is the server's reply to the client
##### HTTP Status codes



















    
