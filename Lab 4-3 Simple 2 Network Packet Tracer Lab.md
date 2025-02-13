# Lab 4-3 Simple 2-Network Packet Tracer Lab

This lab aims to demonstrate how to connect 2 networks together.

### Notes:

Connect laptop/server to switches and switches to router (FastEthernet ports on Router) and pay attention to the interfaces you use

Network address for Foster is 192.168.3.0/24 and Network address for Skiff is 192.168.1.0/24

On CNCS Router:

Router Interfaces are OFF by default. Be sure to click the ON box in the upper right hand corner (in the CLI this is typing no shutdown)

Assign the IP 192.168.3.1 and subnet mask 255.255.255.0 to the Interface connected to the Foster Network

Assign the IP 192.168.1.1 and subnet mask 255.255.255.0 to the Interface connected to the Skiff Network

Configure IP's subnet mask and Default Gateway on the Laptop and Server

On the Laptop assign 192.168.3.20, mask 255.255.255.0 and 192.168.3.1 as the Gateway
On the Server assign 192.168.1.40 Mask 255.255.255.0 and 192.168.1.1 as the Gateway
Once completed, ping server from laptop


![{4394913E-E417-4F64-BEBD-E268172FFA2C}](https://github.com/user-attachments/assets/5aac19c6-e584-4563-a4e7-56549f214c48)

 

Traffic Analysis in Packet Tracer

Go into "Simulation Mode" in Packet Tracer (stopwatch on lower right)

 From Laptop - open up "Web Browser" on Laptop Desktop

Enter the IP address of server and hit "go"

Use Capture/Forward to send to packets hop-by-hop

Continue until you see HTTP Packets in the Simulation Panel

Review Packet Details of a HTTP Packet in the Simulation Panel

![{6ED792F6-4DE0-41B5-B6D6-49374AF910FC}](https://github.com/user-attachments/assets/28c81774-af76-4aae-92d5-00f796c37e35)


Practice Saving Router config

Go back to Real-Time mode (clock)

From Router: Config Tab: Save NVRAM

From Router: Got to "Physical Tab" and use power button to turn off router. 

Power back on by clicking the button again

Use Fast Forward button to get links back

Check router to make sure Interface IP's are still there


![{DEBFA09A-037D-4AAC-91D2-F0F9585E91BE}](https://github.com/user-attachments/assets/77458ee3-9f50-4a44-b56b-2474deb433d7)
