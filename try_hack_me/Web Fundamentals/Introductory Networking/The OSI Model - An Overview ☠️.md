# The OSI Model - An Overview

**OSI (Open System Interconnection)**  Model is standardised model which which we use to demonstrate the theory behind the computer networking.

---
** OSI Model is consist of 7 layers ** :
##### OSI Model

||
--|--|
- **Application**|
- **Presentation**|
- **Session**|
- **Transport**|
- **Data Link**| 
- **Network**|
- **Physical**|
---
#### Layer 7 - Application
- Essentially provides networking options to programs running on computers 
- Exclusively works with Application, providing interface to them to use in order to transmit data.
- When data is given to application layer it passed down into the **Presentation layer**.
---
#### Layer 6 - Presentation 
- Presentation Layer receives data from application layer.
- This data tends to be in format that the application  can understand.
- It's not necessarily standardised format that could be understood by the application layer in the receiving computer.
- Presentation layer translates data into standardised format, **encryption handling**, **compression** or other transformation to the data. 
- With this complete data is passed down to the session layer.
---
#### Layer 5 - Session
When session layer receives correctly formatted data from presentation layer,
- It looks to see if it can setup a connection  with the other computer across the network.
	- If it can't then it sends back an error and process goes no further.
-  If session can establish a connection then job of session layer maintain it.
-  As well as co-operate with the session layer of the remote computer in order to synchronize communications.

--- 
==It's in SESSION Layer== 
- Session layer is particularly important as the session that it creates is unique to the communication in question. 
- Allows to make multiple requests at different endpoints simultaneously without mixing all data ==think about opening two different tabs in your browser at same time.==  
- When the session layer successfully logged a connection between the remote and host computer the data is passed down to Layer 4 : **Transport Layer**
---
#### Layer 4 - Transport 
Transport layer serves numerous important functions.
- It's first purpose is to choose protocol over which the data is to be transmitted.
- The two most common protocols are :
	- [ ] TCP ==Transmission Control Protocol== 
	- [ ] UDP  ==User Datagram Protocol==
---
##### TCP or Transmission Control Protocol
- Transmission is *connection-based* 
- Connection based means that a connection between the computers is established and maintained by for the duration of request.  
- This allows for reliable transmission, as the connection can be used to ensure that the packets all get to the right  place. 
- TCP connection allows two computer remain in constant communication to ensure data can be sent at an acceptable speed and that any lost data is re-sent.
---
#### UDP or User Datagram Protocol
- The opposite is *true*
- Packets of data are essentially thrown into receiving computer.
	- If it can't keep up then that's it's problem ( this is why skype video pixelated if the connection is bad. )
---
> **TCP** would be chosen  for situations where accuracy is favoured over time (e.g-> file transfers, loading web pages)
> 
> UDP is used where speed is most important. (e.g-> video streaming)
---

With a protocol selected  transport protocol divides transmission up into bite-sized pieces (over TCP these are **segments** UDP these are called **datagrams**) , which makes it easier  to transmit message successfully.

---

#### Layer 3 - Network Layer
-  The network layer is responsible for locating destination of your request.
> When you request information from web page then it's network layer that takes IP address for the page and search for the best route to take.
---
#### Layer 2 - Data Link Layer
- The data links focusing on physical addressing of the transmission.
-  It receives a packet from  network layer (that includes IP address for the remote computer )  and Adds in the physical in the Physical (MAC) address of the receiving endpoint. 
-  Inside every network enabled computer is a **Network Interface Card (NIC)**, which comes with a unique **Media Access Control**(MAC) address to identify it.
---
==Some points on MAC Address==
-  MAC address can be set by Manufacturer and literally burnt into the cards , They can't be changed although they can be spoofed.
-  When information is send across a network , it's actually physical card that is used to identify where exactly  to send the information.
-  Additionally Job of data link is to layer is to present the data in format that is suitable for transmission.
-  When data link receives data , as it checked the received information is not corrupted during transmission.
---

#### Layer 1 - Physical Layer
- The physical layer is right down to the hardware of computer.
- This is where electrical pulses that make up data transfer over a network are sent and received. 
- Job of Physical layer is to convert binary data of transmission into signals and transmit them into across the network as well as receiving the incoming signals and convert them into binary data .
---




























