# Encapsulation

As the data passed down in each layer more information containing details specific to the layer in question  is added to the start of transmission.

---

![[Pasted image 20211031072047.png]]

---

The data link also adds the  piece on at the ends of the transmission which is used to verify that the data has not been corrupted on transmission. 

The whole process is called **Encapsulation**.  

---

#### Data has different name at different stage :
- At stage 7,6,5 data is referred as data.
- In transport layer the encapsulated data referred to as **segment/Datagrams**
- In the network layer data is referred as **packet**.
- In the data-link layer packets are referred as **frames**. 
- It's transmitted across network the frame has broken down into bits.

---
>When the message sent on second computer the process is reversed, start from Physical to application.

*The reversing process is called de-encapsulation*.

