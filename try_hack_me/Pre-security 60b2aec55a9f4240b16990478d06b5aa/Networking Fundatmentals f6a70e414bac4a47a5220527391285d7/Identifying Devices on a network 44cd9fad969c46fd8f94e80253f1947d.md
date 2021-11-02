# Identifying Devices on a network

Device can be found by two things :

1. An IP address
2. An Media Access Control (MAC) Address – think of it as a serial number.

### IP Address

An IP (Internet Protocol) address can be used a way of identifying host on a network for a short period of time , Where IP address can be associated with another device without the IP address changing.

[[Pasted image 20210915210845.png]]

IP address can be changed device to device but cannot be active simultaneously more than once within the same network.

IP address follow a set of standards known as protocols . These protocols are the backbone of networking and force many devices to communicate in same language.

**Public address** is used to identify the device on the network **Private address** is used to identify a device amongst other devices.

Public IP address are given by **Internet Service Provider(ISP)**

## MAC Address

Devices on a network will all have physical network interface, which is a microchip board found on the device’s motherboard. This network interface is assigned a unique address at the factory it was built called a MAC address. Mac address is twelve character hexadecimal number Split into two’s and separated by colons.

[[Pasted image 20210915213138.png]]

The MAC address can be faked or **spoofed** in a process known as spoofing. ### Ping (ICMP)

Ping is a most fundamental tool . Ping uses **ICMP(Internet Control Message Protocol)** packets to determine the connection performance between the devices.