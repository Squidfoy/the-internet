# How does the internet work digitally?
Digitally, the internet trasfers data using **packets** and **protocols**.  
### Packets
A **packet** is a small piece of a larger set of data. You can think of packets as puzzle pieces that make up a larger puzzle. When data gets sent over the internet, it is broken up into these packets for the transfer and then reassembled at the destination.  
  
If all the packets are sent separite from eachother, how does the recieving computer know how to piece them together? Each data set is sent with a *header*, which is sent bef USore all of the packets. The header contains information about the packets contents and also helps the recieving machine know what to do with the packets. The header acts as the instructions so that the recieving computer can reassemble and use the packets as efficiently as possible.  
  
Why use packets instead of transfering the entire data set? Some pieces of data are quite large, and trasferring it all at once would take a lot of time and may block the internet connection for others. Using packets allows data transfer to go more efficiently, decreasing network congestion and increasing transfer speed. Additionally, if any of the packets fail to send, the recieving computer is only missing part of the data rather than the entire data (and the missing packet can be sent again).
  
Packets are sent across the internet and then reassembled at their destination, but the packets don't all send through the same connection. A process called *packet switching* is used to send packets across the internet. This means that, as the packets are being sent, many different routers and switches (which we will learn about in the next section) are used in the process. This process is, once again, used to increase efficiency. If we tried to send all of the packets along the same connection, the data transfer would take much too long and would not allow for many people to use the internet at the same time.  
![Packet switching pic](https://github.com/user-attachments/assets/6ad98851-ddb5-4d66-90ac-e41bddbe1d7a)  
### Protocols
Protocols allow computers to connect and transfer data even if they use different hardware and software. A **protocol** is a stanardized way of formatting data and doing certain actions so that multiple devices are able to communicate.  
Some different protocas include TCP, UDP, and IP.  
  
#### Internet Protocol (IP)
IP is the protocal that oversees sending packets from network to netork. IP requires each packet to have IP information attatched to it, or an IP address. This helps rounters send the packets to the right place. Packets aren't the ontly thing with an IP address, every domain (or website) and physical device that connects to the internet has its own IP address. IP addressing allows data to get transfered to the right place every time, which is just what a protocol is meant to do.
  
#### Transmission Control Protocol (TCP)
IP ensures that the packets arrive at the correct destination, but it does not guaranteee that, when they get there, they are in the correct order and are devoid or errors. It is the responsibility of TCP to identify errors and put the puzzle of packets back together. TCP retains the connection with the sender before the first packet is sent and after the last one arrives. If any packets are missing, it asks the sender to resend that particular packet. TCP manages to do its job through a process called the *3-way handshake*. 
1. SYN: The sender sends an initial request packet in order to begin the line of communication.
2. SYN-ACK: The reciver sends back a packat acknowledging the request.
3. ACK: The sender sends another packet to confirm the process and oficially establish a connection.  
Once the 3-way handshake is complete, the packets of data can be sent. When they have been reassembled without error, the connection is broken.
  
TCP is used with IP (TCP/IP) to efficiently send data across the internet.
  
#### User Datagram Protocal (UCP)
  
Click [here](README.md) to go back to the main page.
