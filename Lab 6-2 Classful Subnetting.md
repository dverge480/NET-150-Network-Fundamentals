# Lab 6-2 Classful Subnetting

This lab aims to demonstrate how to properly subnet a network.

### Notes:

It is important to document the IP addresses of each router.

Label each subnet, and then give each router the first available address of the subnet. Remember to also assign these as the default gateways of each respective subnet.

Once this is set up, ping the devices in each subnet from a device within that subnet to test connectivity.

Use Serial DCE to connect the routers, and use available IPs to map them to the network. Remember to turn on the port through the router. Utilize RIP to set the clock rate to 64000.


![{B75DCA2E-0A9C-49F4-9F9C-8A017C36895D}](https://github.com/user-attachments/assets/4ab1967e-1951-4f34-85e3-c5c526b8ceef)


This is what a successful ping from devices on each subnet should look like after completing the steps above.


![{D83139C7-E3A2-4E0F-A549-2A77792805CE}](https://github.com/user-attachments/assets/e4695c1e-f966-4126-922a-3b60e31a4451)



This is what a successful ping from the remaining subnet should look like.

The first ping from any device will almost always fail. If it continues to fail, make sure that your default gateways are properly configured.

The most difficult part of this lab is keeping track of what IPs are assigned to each device. This highlights how important documentation is in networking and cybersecurity.
