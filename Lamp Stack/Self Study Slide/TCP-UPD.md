# WHAT IS TRANSMISSION CONTROL PROTOCOL(TCP): 
TCP is one of the core protocols of the Internet Protocol (IP) suite. It operates at the Transport Layer and is used to establish a reliable and ordered transmission of data between devices on a network. TCP ensures that data sent from one device arrives intact and in the correct order at its destination.
  ## Key Characteristics of TCP:
  #### Connection-Oriented:
TCP requires a connection to be established between the sender and receiver before data can be transmitted. This is done through a process called the three-way handshake.
  #### Reliable Data Transfer:
TCP ensures that all data sent is received correctly and in the proper sequence. If packets are lost, duplicated, or received out of order, TCP will retransmit and reorder them as needed.
  #### Error Checking and Correction:
TCP uses checksums to detect errors in the data. If an error is found, the affected packets are retransmitted. This ensures the integrity of the data being transmitted.
  #### Flow Control:
TCP manages the rate of data transmission between the sender and receiver using a mechanism called sliding window. This prevents the sender from overwhelming the receiver with too much data at once.
  #### Congestion Control:
TCP adjusts the rate of data transmission based on the current state of the network, preventing congestion and ensuring efficient use of network resources.
## How TCP Works:
  #### Three-Way Handshake:
Before data transmission, TCP establishes a connection between the sender and receiver using a three-step process:
SYN (Synchronize): The sender sends a synchronization request to the receiver.
SYN-ACK (Synchronize-Acknowledge): The receiver acknowledges the request and responds.
ACK (Acknowledge): The sender acknowledges the response, and the connection is established.
  #### Data Transfer:
Once the connection is established, data is broken down into smaller packets, each with a unique sequence number. The receiver acknowledges each packet received. If a packet is not acknowledged, it is retransmitted.
  #### Connection Termination:
When the data transfer is complete, the connection is terminated using a four-step process involving FIN (finish) and ACK packets. This ensures both parties agree to close the connection.
## Use Cases of TCP:
  #### Web Browsing (HTTP/HTTPS): 
  TCP ensures that all elements of a webpage are delivered correctly, including text, images, and scripts.
  #### Email (SMTP, IMAP, POP3): 
  Guarantees that emails are sent and received without loss.
  #### File Transfer (FTP): 
  Ensures that files are transferred completely and accurately.
  #### Remote Access (SSH): 
  Provides secure and reliable connections for remote management of devices and systems.
## Example:
When you visit a website, your browser uses TCP to connect to the web server. The server sends the website's content in a series of TCP packets. If any packets are lost or corrupted, they are retransmitted, ensuring that you receive the complete and correct webpage.
## Summary of TCP Features:
  #### Reliability: 
  Guarantees data delivery and order.
  #### Connection-Oriented: 
  Requires establishing a connection before data transfer.
  #### Error Checking: 
  Uses checksums and retransmission to ensure data integrity.
  #### Flow and Congestion Control: 
  Manages data flow and adapts to network conditions.
In summary, TCP is a robust and reliable protocol designed for scenarios where data integrity and order are crucial, making it a foundational element of many Internet services and applications.
## WHAT IS USER DATAGRAM PROTOCOL (UDP): 
It's a communication protocol used in the Internet Protocol (IP) suite, specifically at the Transport Layer. UDP is known for its simplicity and speed, as it provides a way to send data across a network without establishing a connection or ensuring reliable delivery.
## Key Characteristics of UDP:
  #### Connectionless: 
  UDP does not establish a connection before sending data, which means it sends packets directly to the recipient without a handshake process.
  #### Unreliable: 
  There is no guarantee that the data will reach its destination. If packets are lost or arrive out of order, they are not retransmitted.
  #### No Error Checking or Correction: 
  UDP does not check for errors or correct them, unlike TCP. This means there is no mechanism to ensure that all data arrives intact and in the correct order.
  #### Low Overhead: 
  Because it lacks the features of error checking and connection management, UDP has less overhead, making it faster and more efficient for certain types of communication.
## How UDP Works:
  #### Data Transfer: 
  Data is sent in small chunks called datagrams. Each datagram is sent independently and can take different paths through the network.
  #### No Acknowledgment: 
  The sender does not receive any confirmation from the receiver that the data has been received, making the protocol lightweight.
## Use Cases of UDP:
  #### Streaming Media: 
  Used for real-time video and audio streaming where minor data loss is acceptable, but low latency is critical.
  #### Online Gaming: 
  Ensures quick transmission of data, which is crucial for fast-paced games, even if some packets are lost.
  #### VoIP (Voice over IP): 
  Ensures smooth, real-time voice communication with minimal delay.
  #### DNS (Domain Name System): 
  Sends short queries and responses quickly without the need for a connection.


## Example:
When watching a live sports stream, UDP is often used because a minor glitch or data loss will not significantly impact the experience. The priority is on continuous data flow and low latency, rather than ensuring every packet arrives.
In summary, UDP is an efficient and fast protocol, suitable for applications where speed is more critical than perfect data integrity.

![image](https://github.com/user-attachments/assets/c7565b84-8505-4f2d-a9f8-beda06c5e172)

## LIST OF COMMON PORTS COMMONLY USED IN WEB
Here are the most commonly used ports for various web and network protocols:
  ### HTTP (Hypertext Transfer Protocol):
  #### Port 80: 
  The default port used for non-secure HTTP web traffic.
  ### HTTPS (Hypertext Transfer Protocol Secure):
  #### Port 443: 
  The default port used for secure HTTPS web traffic, which encrypts data using SSL/TLS.
  ### SSH (Secure Shell):
  #### Port 22: 
  The default port used for secure remote login and command execution on networked devices.
  ### Telnet:
  #### Port 23: 
  The default port used for unsecure remote login and command execution. Telnet is not recommended for secure communication as it transmits data, including passwords, in plain text.
  ### FTP (File Transfer Protocol):
  #### Port 21: 
  Used to establish the initial connection and control communication between the client and server.
  #### Port 20: 
  Used for data transfer in active mode FTP.
  ### SFTP (SSH File Transfer Protocol):
  #### Port 22: 
  Unlike FTP, SFTP operates over the SSH protocol and uses the same port as SSH for secure file transfer.


