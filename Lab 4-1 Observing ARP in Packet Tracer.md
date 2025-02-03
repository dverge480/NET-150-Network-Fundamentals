# Lab 4-1 Observing ARP in Packet Tracer

This lab aims to gain some more exposure to Address Resolution Protocol and Ethernet and develop a deeper understanding of the relationship between these two protocols.

### Notes:
Use the Devices Section in the lower left to build a simple network diagram using 4 generic computers and a switch
Select the Device Category, locate the device you want, and click-drag into the workspace
Do not connect the computers to the switch yet.

What is the MAC address of the ethernet adapter on PC0? 00E0.B01B.35BE
Is there an IP address? No

Hold the mouse over the switch to see the configuration.
Are there IP addresses assigned? No

Click on PC0 - Desktop Tab
Open the Command Prompt 
Type arp  –a to  see the arp table and review to see if there are any entries
Assign IP addresses to the computers (use 4 addresses on the same network : 10.10.10.X) What does it mean for PCs to be "on the same network"? It means that computers share the same network address.

Click on the switch and the select CLI.   This is the Command Line Interface.   You need to get to the root CLI prompt which looks like Switch#
- If the prompt looks like:  Switch>,  then type enable to enter admin mode
- If the prompt looks like  Switch (config)#  type exit to get back to the basic mode for admin
Then type show mac-address-table

The "Lightning Bolt" in lower left will allow you to add connections between devices
Use the straight black cable (ethernet straight-through) to connect PC0 to Fa0/10 on the switch, PC1 to Fa0/11

On PC0, open the Desktop and select Command Prompt.
From the command prompt on PC0, ping PC3 using it’s IP address.
![{7B4C4651-CFA0-49E7-B16F-23CB9BA8A32D}](https://github.com/user-attachments/assets/a6deb8eb-f48f-480f-a234-8ded06b02880)


Examine the address table of the switch again.
![{D10ACCB7-63A1-4DD4-ABBB-7CC0D0C0A503}](https://github.com/user-attachments/assets/c691848d-bcd8-4ec9-a8d9-61dc0c1de83e)

The finished network architecture should look like this:
![{3B7BB719-F8D4-4B0D-AD45-639BBE5C85E0}](https://github.com/user-attachments/assets/07b9e9ef-01eb-41b6-8858-a4b1d1d67e5c)







