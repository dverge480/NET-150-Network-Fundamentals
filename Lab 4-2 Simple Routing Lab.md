# Lab 4-2 Simple Routing Lab

This lab aims to demonstrate how to configure and observe a simple routed network.

### Notes
PC0
IP address: 192.168.1.10
Subnet Mask: 255.255.255.0
PC1
IP address: 192.168.2.20
Subnet Mask: 255.255.255.0
PC2
IP address: 192.168.3.30
Subnet Mask: 255.255.255.0

To set the gateway for a PC, choose the Config tab, and then choose 'Settings' in the left-hand menu. You can enter the gateway IP in the 'Gateway' field (make sure the 'Static' button above it is selected).

A default gateway is a device that is the point of contact for all network traffic.


PC0: 192.168.1.1
PC1: 192.168.2.1
PC3: 192.168.3.1

Click on the multilayer switch, choose the Config tab in the window that appears, and then pick the FastEthernet interface that you want to configure (in the example below, we're selecting FastEthernet0/1).

FastEthernet0/1: 192.168.1.1
FastEthernet0/2: 192.168.2.1
FastEthernet0/3: 192.168.3.1
All subnet masks will be 255.255.255.0
Once all of the interfaces are configured, try pinging PC1 and PC2 from PC0.


![image](https://github.com/user-attachments/assets/d2bedb3a-9087-4026-b897-44c7592596c3)


![image](https://github.com/user-attachments/assets/f068554c-a740-4a9d-8bc6-91ce7e1fb63a)

### Part 2

Click on the Simulation button in the bottom-right corner of the Packet Tracer window.

A Simulation panel will appear on the right side of the window. Since Packet Tracer will simulate many protocols by default, click the 'Show All/None' button at the bottom of this window, and then click the 'Edit Filters' button. Check the ICMP box in the IPv4 tab of the window that pops up.

Now, ping PC1 from PC0. The initial ping packet should appear in the simulation window. Click the '►|' button a few times until the packet reaches PC1 - you should see the following packets in the simulation window:


![image](https://github.com/user-attachments/assets/6e0b2324-5b9d-47d3-be18-81de1a1552d3)

If you click on the packet at the Multilayer Switch, you'll receive a summary of the OSI information the packet contains as it both arrives at and leaves the switch. In particular, at layer 2 you'll see something like 'AAAA.AAAA.AAAA >> BBBB.BBBB.BBBB' - this indicates that the packet is being sent from the MAC address AAAA.AAAA.AAAA to the MAC address BBBB.BBBB.BBBB. If you click on the Inbound and Outbound detail tabs, you can see how this information is specifically formatted within each packet.

What is the Source and Destination MAC address of the packet as it arrives at the switch? (1 point)

![image](https://github.com/user-attachments/assets/53f8c4bc-9706-452d-a1e2-26483fbdd807)


What is the Source and Destination MAC address of the packet as it leaves the switch? (1 point) 


![image](https://github.com/user-attachments/assets/cc2ead83-fadd-4eaa-be90-640f32240bfd)


Why does the Destination MAC of the packet arriving at the switch match the Source MAC of the packet leaving the switch? (3 point) 
This is because the ping is simply returning a reply to where the packet initially came from, signaling to the sender that the connection was successfully established and functional.
