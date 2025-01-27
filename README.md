# Lab 2-2 Observing LAN Activity 

This lab aims to demonstrate how to observe network traffic on a LAN using the ping process to illustrate a connection.


### Notes:
Typing ICMP in wireshark shows only ping requests and replies

Source mac address is listed in the Ethernet II part of the box

IP Address of Default Gateway: 192.168.1.250
*Use ipconfig /all to find this information

What is the MAC address of your workstation's NIC? What is the MAC address of the Default Gateway Router interface (NIC)?

To find this use ipconfig /all, to find the MAC address of the default gateway, use the netstat -rn command.
-r Shows the routing table
-n Shows IP addresses and ports in numeric form
Then, use the arp -a to display the ARP table, which maps IP addresses to MAC addresses.
![{3A08BDD7-23FB-4419-ACCC-54A559385A8C}](https://github.com/user-attachments/assets/bb2cc018-43db-43bf-85f5-e0206db8aa40)


MAC: 1C-69-7A-A6-49-2B
MAC of Default Gateway: 00-00-5e-00-01-ca
![{B5EBE442-1253-43A3-9017-414AEB1CDFC7}](https://github.com/user-attachments/assets/3094581e-a82a-4dfb-bf69-43bf2e2f7919)

What are the source and destination MAC addresses of the ICMP:
![{B8D04A98-398E-40DE-BF99-C13710A48D04}](https://github.com/user-attachments/assets/e58cf8f7-47de-4db4-ab1e-f1f8d65b76a8)

Request - Source: 1c:69:7a:a6:49:2b Destination: 00:00:5e:00:01:ca
![{3F3AFF37-8669-427C-A084-ED1FF27EF742}](https://github.com/user-attachments/assets/4230ce23-3fc6-486f-a7e0-9a29630faf10)

Response - Source: 0c:59:9c:f7:de:30 Destination: 1c:69:7a:a6:49:2b

### Part 2

IP Address of www.timeslive.co.za: 142.250.80.19
![{3FA1CA19-FB6E-4DAC-A433-1AF060F16E05}](https://github.com/user-attachments/assets/00529410-3d51-4151-aa43-276162bcd804)

What are the source and destination MAC addresses of the ICMP:

Request - Source: 1c:69:7a:49:2b Destination: 00:00:5e:00:01:ca
![{4E1C75A5-EF85-4EA9-BA13-E95D5A5AA36D}](https://github.com/user-attachments/assets/f04e1fd2-03cb-470d-a08b-1c614105e753)

Response - Source: 0c:59:9c:f7:de:30 Destination: 1c:69:7a:a6:49:2b
![{89C34617-AFB9-4CD1-8D3F-B0E5538447A5}](https://github.com/user-attachments/assets/f56a278a-d9b3-49a8-9c03-d47ee39ebcb1)

They are the same as above, which is an indicator of Proxy ARP usage.
