# Lab 3-2 Exploring Broadcast Domains


This lab aims to demonstrate the process of exploring and understanding broadcast domains on Layer 2.

### Notes:

Start a wireshark capture and then ping the Google Public DNS server (8.8.8.8), then stop the capture. Analyze the ICMP response.

What is the source MAC address? What is the destination MAC address? (Hint: Data Link Layer Header)
Source MAC Address: 4c:6d:58:1a:df:3c Destination MAC Address: 74:56:3c:46:34:b4 

Does the source MAC address look familiar from prior labs? Do you think it is the Google Server's MAC address? 

Yes it is similar because it is the same source/destination used to ping google in the previous labs. MAC addresses do not change on a piece of hardware. It can’t possibly be Google’s MAC address, as we could only know that if we hacked google.

### Part 2

Ping a neighboring machine's IP address, and record the source and destination MAC of the ping reply.

Neighboring IP: 192.168.1.32				Source IP: 192.168.1.123
Neighboring MAC: 74-56-3C-46-34-B4		Source MAC: 1C-69-7A-A6-49-2B

Information according to Wireshark:

Neighboring IP: 192.168.1.32				Source IP: 192.168.1.123
Neighboring MAC: 74-56-3C-46-34-B4		Source MAC: 1C-69-7A-A6-49-2B
Detected MAC: 74:56:3c:46:34:b4			Detected MAC: 1c:69:7a:a6:49:2b


Does the MAC address match the address from your traffic capture? If not - what do you think happened?

The MAC addresses all match the actual MAC addresses found using ipconfig /all on both machines. Since it did not change, I can infer that the ping took no hops from one LAN to another, because if it did, one of the MAC addresses would be that of a router.


### Part 3
Start a Wireshark capture on both PCs and let it run, ping your partner's IP address
Stop the captures on both Workstations, find and compare the ICMP traffic on both devices

The source and destination MAC addresses are the same when reviewed in Wireshark from both devices. This is because MAC addresses cannot be changed and are the physical address on a LAN.

