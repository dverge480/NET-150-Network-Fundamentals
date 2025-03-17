# Lab 9-1 Stating Routing #1

This lab aims to demonstrate what happens to a network and routing when connecting multiple or new users.

### Notes:

#### The following information is related to PC0:
IP Address: 192.168.30.3
Default Gateway: 192.168.30.1
Can PC1 be pinged?: Yes
Can PCs 2-5 be pinged?: No

#### Why do pings to other networks fail? 
The network cannot travel farther than its own because further routing is not set up.

### Create Static Routes:

On R1, go into "config" mode
Reminder: Go to CLI, type "enable" and then "config terminal"
Then enter:

R1(config)#ip route 192.168.30.0 255.255.255.0 10.10.20.2 

R1(config)#ip route 192.168.10.0 255.255.255.0 10.10.10.2

This provides routes to Network 3 and Network 1 respectively
On R2, go into "config" mode and enter

R2(config)#ip route 192.168.10.0 255.255.255.0 10.10.20.1 

R2(config)#ip route 10.10.10.0 255.255.255.0 10.10.20.1 

R2(config)#ip route 192.168.20.0 255.255.255.0 10.10.20.1 

On R3, based on what you have configured for R1 and R2, what do you think the configuration should be for R3?

R3(config)#ip route 192.168.30.0 255.255.255.0 10.10.10.1

R3(config)#ip route 192.168.20.0 255.255.255.0 10.10.10.1

R3(config)#ip route 10.10.20.0 255.255.255.0 10.10.10.1

Now the network should be completely functional 



![{E3429C15-3645-4D7F-8642-DF3E634C001A}](https://github.com/user-attachments/assets/5c2f75e8-539d-44ba-b141-bc349c27f29c)



#### What does the show ip route command do?

It basically shows all routes, how they are connected, and the connection information. This is useful for troubleshooting a network.

#### Imagine a larger network with 25 different network segments (subnets). What would the challenge be with using "static routes"? 

Using static routing, a larger network would be tremendously exhaustive to set up for a network administrator. Networks constantly change, and static routing isn’t necessarily the most fault tolerant. Also, there is minimal scalability due to the work that must be done to route the network by hand.
