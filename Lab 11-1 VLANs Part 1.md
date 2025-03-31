# Lab 11-1: VLANs Part 1

This lab aims to demonstrate how to set up and configure VLANs in Packet Tracer.

### Notes:


### Configure Switch Ports for VLANs:

On 1st Floor Switch, Go to Config/VLAN Database and add the VLANs the switch will support:
VLAN Number: 10 Name: ENG
VLAN Number: 20 Name: MKT
VLAN Number: 30 Name: ACT

Then, configure which ports are in which VLAN from Config tab by changing the VLAN number for the Access Port configuration per interface
FastEthernet 0/1 can be VLAN 10 (ENG)
FastEthernet 0/2 can be VLAN 20 (MKT)
FastEthernet 0/3 can be VLAN 30 (ACT)

Then, configure the Trunk port that will be used to connect the switch to the 2nd Floor Switch
GigabitEthernet 0/1 change to Trunk and add VLANs 10, 20, and 30 (leaving the other default VLANs checked is fine)

Repeat 1-3 on 2nd Floor and 3rd Floor switches

Note: On 2nd Floor switch, you will need to configure both GigabitEthernet 0/1 and Gigabit/Ethernet 0/2 as Trunk ports (step 3) as it connects to two switches

### Connect Devices

Assign Appropriate IP configurations to the PC's
ENG network is 192.168.10.0/24 and the default gateway will be 192.168.10.1
MKT network is 192.168.20.0/24 and the default gateway will be 192.168.20.1
ACT network is 192.168.30.0/24 and the default gateway will be 192.168.30.1
Remember, every PC needs a unique address
Connect PC's to the switch on their floor.
Make sure to connect the PC to the Port on the switch that is in their VLAN!
Connect switches to each other using Crossover Cables  and the configured Trunk ports
If everything is connected and addressed correctly
All PC's on the same VLAN should be able to ping each other
But, PC's on different VLANs (even on the same switch) should not be able to ping
At this point, All PC's on the same VLAN should ping one another - BUT PC's on different VLANs should not be able to ping one another


![{A4606B12-B4B6-49C4-A4CE-2ECBB83239EE}](https://github.com/user-attachments/assets/fced69a1-2e45-47b9-ae17-c96bd794c7d4)


PC’s on different VLANs cannot ping each other because each VLAN is a different, secluded segment of broadcast traffic that is limited to specific endpoints. 
