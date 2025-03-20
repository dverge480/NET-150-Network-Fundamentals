# Lab 9-2 Static Routing #2

This lab aims to demonstrate how to subnet a large number of users on a network and configure static routing properly.

### Notes



![{A9D803AE-425E-4F4A-ADB5-4159605FF846}](https://github.com/user-attachments/assets/2571e6c3-05d7-43a2-a0c9-fdb70d163eb9)


When SalesWest tries to ping SalesEast, the packet is in the serial port but does not have any direction on where to go. Since, SalesWest and SalesEast are on different networks, this is where static routing comes into play.

To add static routing, enter the network address, the subnet mask, and the next hop which would be the router’s serial connection interface.

The command should be formatted like this: (IP address of network you are trying to ping TO) (Subnet Mask of that network) (IP address of the serial interface on the receiving router)

After entering all of the possible routes into the routers, a ping from both routers should work.

![{3778BB93-8CA4-4ABA-A50D-958B5FBD7700}](https://github.com/user-attachments/assets/3174d53e-1102-45db-ba30-fb5f8010bc65)


