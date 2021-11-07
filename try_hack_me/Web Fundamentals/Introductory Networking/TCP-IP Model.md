# TCP/IP Model
-  It's very similar to OSI Model. It's very few years older and serves as the basis for real world networking.
-  The TCP/IP model consists of four layer
	1. Application
	2. Transport 
	3. Internet
	4. Network Interface

![[Pasted image 20211031074942.png]]

> The process of encapsulation and de-encapsulation work in exactly same way with th TCP/IP model as they do with the OSI Model.

- TCP which controls flow of data between two endpoints.
- Internet Protocol(IP) which controls how packets addressed and sent.

## TCP
- TCP is connection based protocol.
- In other words, before you send any data via TCP you must first form a stable connection between two computers.
> The process of forming this connection is called three-way handshake.

## Setting Up Connection
Computer first send a special request to the remote server indicating that it wants to initialise a connection.
- This request contains something called a **SYN(synchronise)** bit, which essentially makes first contact in starting the connection process.
![[Pasted image 20211031083544.png]]
- The server will then respond with a packet containing a **SYN** bit as well as another *acknowledgement* bit, called **ACK**.
- Finally, your computer will send a packet that contains **ACK** bit by itself, confirming that connection has been setup successfully.

With three way handshake successfully completed, data can be reliably transmitted between the two computers. 

>Any data that is lost or corrupted during transmission is re-sent, that's why this connection is lossless.




