# Intro to LAN

# LAN Topologies

**Topology** is the design of networking at the hand.

## Star Topology

The main thing is devices are connected to the Central networking device such as Switch or hub.

This topology commonly found today because of it’s reliability and scalability or despite the cost.

Any information sent to a device in this topology is sent via the Central device to which it connects.

---

### ADVANTAGES & DISADVANTAGES

- More cabling and the purchase of dedicated networking equipment in this topology. It’s more expensive than any other topologies.
- This topology scalable in Nature, which means that it’s very easy to add more devices as the demand for the network increases.
- More the network scales more the maintenance required to keep the network functional.
- Further more star topology is prone to failure , abeit reduced.

If the Central hardware that connects devices fails there devices will no longer be to receive or send data . Thankfully the centralised hardware are often robust.

## Bus Topology

This type of connection is relies upon a single connection which is known as backbone cable. This type of topology is similar to leaf off from a tree.

### ADVANTAGES & DISADVATAGES

- Because all data destined for each device travel along the same cable; it is very quickly to prone becoming very slow and bottlenecked if devices within the topology simultaneously requesting data.
- The bottleneck also results in very difficult troubleshooting because its quickly become difficult to identify which device is experiencing issue with data all travelling in the same route.
- It’s become most easy and cost-efficient topologies to setup because of their expenses.
- If there is any single point of failure in cable or backbone the system does not work.

## Ring Topology

The ring topology is also known as token topology boasts some similarities. Devices and computers are directly connected to each other to form a loop meaning that there is a little cabling is required and less dependence on dedicated hardware required such as within a star topology.

### ADVANTAGES & DISADVANTAGES

- A ring topology works by sending data across the loop until it reaches the destined device, using other devices along the loop to forward the data. Interestingly, a device will only send received data from another device in this topology if it does not have any to send itself. If the device happens to have data to send, it will send its own data first before sending data from another device.
- Because there is only one direction for data to travel across this topology, it is fairly easy to troubleshoot any faults that arise. However, this is a double-edged sword because it isn’t an efficient way of data travelling across a network, as it may have to visit many multiple devices first before reaching the intended device.
- Lastly, ring topologies are less prone to bottlenecks, such as within a bus topology, as large amounts of traffic are not travelling across the network at any one time. The design of this topology does, however, mean that a fault such as cut cable, or broken device will result in the entire networking breaking.

### What is a SWITCH

Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet. These various devices plug into a switch’s port. Switches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network. Switches can connect a large number of devices by having ports of 4, 8, 16, 24, 32, and 64 for devices to plug into.

Switches are much more efficient than their lesser counterpart (hubs/repeaters). Switches keep track of what device is connected to which port. This way, when they receive a packet, instead of repeating that packet to every port like a hub would do, it just sends it to the intended target, thus reducing network traffic.

Both Switches and Routers can be connected to one another. The ability to do this increases the redundancy (the reliability) of a network by adding multiple paths for data to take. If one path goes down, another can be used. Whilst this may reduce the overall performance of a network because packets have to take longer to travel, there is no downtime – a small price to pay considering the alternative.