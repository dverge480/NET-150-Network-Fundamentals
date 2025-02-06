# Lab 3-1 ARP Observation

This lab aims to demonstrate the process of capturing and analyzing ARP (Address Resolution Protocol) requests.

### Notes:

Clear the arp cache command “arp -d” if arp -d does not work try: netsh interface ip delete arpcache

What is the default gateway? 184.171.151.250

Open Wireshark and start a capture, then clear the arp cache again, and ping the default gateway. Stop the capture.

Find the ARP broadcast that your computer used to find the gateway's MAC address.


![Screenshot 2025-02-06 131318](https://github.com/user-attachments/assets/8f3b13b7-3605-4b12-87ed-717a202585b3)


Find the ARP reply from the gateway back to your computer.


![Screenshot 2025-02-06 132707](https://github.com/user-attachments/assets/4c33b110-2588-4d25-838b-924b42b481e1)



What is the message sent in the ARP Request? 

“Who has 192.168.250.1? Tell 192.168.1.32”

 What is the message sent in the ARP Reply?

“192.168.1.250 is at 00:00:5e:00:01:ca”

To add a filter in Wireshark to show ARP traffic only, type “arp” in the filters search bar.

If I ping another system with the IP address of 192.168.1.32 from 192.168.1.123, the response should look like this:


![Screenshot 2025-02-06 133551](https://github.com/user-attachments/assets/2b66e74a-433b-4c56-baf5-823a69cba4ff)



What do you see in the ARP request and reply? Can you discern the MAC address for the google DNS server or not?  Can you explain what happened?

The request and reply are not similar to the previous requests because there is no ARP broadcast to retrieve a physical address, so the filter for Wireshark should be set to ICMP. The MAC address retrieved was only that of a router, not the Google server. To put it simply, the request goes through a router, and MAC addresses can only be retrieved on a LAN.
