# Lab 10-1 Configuring RIP

This lab aims to demonstrate how to configure RIP.

### Notes:

Here is the configuration for R2:
From "config" mode type:
router rip
This will now put you in "router config mode"
Then specify the version with
version 2
And then specify the networks directly connected to Router 2
network 192.168.30.0
network 10.10.20.0

For each router, run network *ip* for each interface touching the router’s interface.
For example, router R1 looks like this:


![{5C3614AD-09B4-4202-8C2E-5640F38AB610}](https://github.com/user-attachments/assets/1e60ed81-f653-4eb1-a3c7-636472defb39)


Run:
R1(config)# router rip
R1(config-router)# version 2
R1(config-router)# network 192.168.20.0
R1(config-router)# network 10.10.20.0
R1(config-router)# network 10.10.10.0

For R3:
R3> enable
R3# configure terminal
R3(config)# router rip
R3(config-router)# version 2
R3(config-router)# network 192.168.10.0
R3(config-router)# network 10.10.10.0
R3(config-router)# exit
R3(config)# exit
R3#

R1 Routing Table:


![{9056E0F7-79A2-46A4-AD7E-42A18E26F83F}](https://github.com/user-attachments/assets/8814a092-b126-437a-93e6-6a55888b7b58)


R2 Routing Table:


![{8B452D29-A0BB-4011-82E2-2BF28AD85853}](https://github.com/user-attachments/assets/ce4ddf6f-1e1d-442b-8945-588e09529db0)


R3 Routing Table:


![{EB9E302B-948A-4DAE-ACF5-8CEB2637C929}](https://github.com/user-attachments/assets/842c76d3-ff31-4205-9731-8a4c84c0145c)


Packet from R1 to R3


![{BC1DDA54-9572-421E-AF2F-DB5EFC486AD3}](https://github.com/user-attachments/assets/180ea225-9a14-49e0-a756-c02bd2d25250)


Packet from R1 to R2


![{12013A02-C81B-403E-AD4A-49EE5E4A1CC6}](https://github.com/user-attachments/assets/42370a89-637f-4b0a-867b-e61663bdb5e9)


