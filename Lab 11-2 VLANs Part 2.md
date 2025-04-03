# Lab 11-2 VLANs Part 2

This lab aims to demonstrate how to further configure VLANs in addition to part 1 of this lab.

### Notes:

On 3rd Floor Switch Only:
Go to Config Tab GigabitEthernet0/1 and change to Trunk
Connect Router interface FastEthernet0/0 to GigabitEthernet0/1 on 3rd Floor Switch using a straight-through cable
Define the VLANs on the Router as you did on the switches
There is an error in the router configuration for the vlan 10 sub which is as follows. There should NOT be a native at the end of the encapsulation and we need to remove it. 
interface FastEthernet0/0.10 native

encapsulation dot1Q 10 

ip address 192.168.10.1 255.255.255.0

To fix this, go to the CLI in packet tracer and type exit until you see Router#. If you see Router> you have typed one too many exits and you need to type enable to get back to privilege mode. 
We need to enter configuration mode for sub-interface Fa0/0.10 and then remove the encapsulation. We will then create an encapsulation without the native and then add the network interface address. 

config t
interface FastEthernet0/0.10
no encapsulation dot1Q 10 native
encapsulation dot1Q 10
ip address 192.168.10.1 255.255.255.0

The commands I ran were:

enable
configure terminal
interface FastEthernet0/0.10
no encapsulation dot1Q 10 native
encapsulation dot1Q 10
ip address 192.168.10.1 255.255.255.0
exit
exit
write memory


![{C718CC65-326B-46E1-8701-137904A08A76}](https://github.com/user-attachments/assets/91fd046a-034b-452e-828a-c49df0d995da)



