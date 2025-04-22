# Lab 12-2 Building a WLAN

This lab demonstrates how to build a WLAN in Cisco Packet Tracer.

### Notes:


### Part 1: Configure a Wireless Router

Step 1: Configure the Internet connection type on the WR.
● Click WR > GUI tab.
● Set the Internet Connection type to Static IP.
● Configure the Internet IP address according to the Addressing Table.

Step 2: Configure the network setup.
● Scroll down to Network Setup. For the Router IP option, set the IP address to the Wireless
Router’s LAN address and the subnet mask
● Enable the DHCP server.
● Scroll to the bottom of the page and click Save Settings.

Step 3: Configure wireless access and security.
● At the top of the window, click Wireless. Set the Network Mode to Wireless-N Only and
change the SSID to whatever you want to call your network.
● Disable SSID Broadcast and click Save Settings.
● Click the Wireless Security option.
● Change the Security Mode from Disabled to WPA2 Personal.
● Configure a passphrase.
● Scroll to the bottom of the page and click Save Settings.

### Part 2: Configure a Wireless Client

Step 1: Configure Laptop1 for wireless connectivity.
Because SSID broadcast is disabled, you must manually configure Laptop1 with the correct SSID
and passphrase to establish a connection with the router.
● Click Laptop1 > Desktop > PC Wireless.
● Click the Profiles tab.
● Click New.
● Name the new profile Wireless Access.
● On the next screen, click Advanced Setup. Leave on Infrastructure Mode
o Then manually enter the SSID of your network on Wireless Network Name. Click
Next.
● Choose Obtain network settings automatically (DHCP) as the network settings, and then
click Next.
● On Wireless Security, choose WPA2-Personal as the method of encryption and click Next.
● Enter the passphrase and click Next.
● Click Save and then click Connect to Network.

Step 2: Verify Laptop1 wireless connectivity and IP addressing configuration.
● The Signal Strength and Link Quality indicators should show that you have a strong signal.
NET 150
● Click More Information to see details of the connection including IP addressing information.

● Close the PC Wireless configuration window.

Step 3: Configure Laptops 2 and 3 to connect to Wireless

### Part 3: Connect to Wired Router and Web Server

Step 1: Configure the Wired Router with the correct IP addresses per the Table
● Connect the Wired Router to the Wireless Router using a crossover cable and correct ports
● Connect the Wired Router to the Web Server using a crossover cable and the correct ports.
Step 2: Access Web server from the Laptops
● Using the Web Browser on the laptops – connect to the Web Server



![Screenshot 2025-04-22 121116](https://github.com/user-attachments/assets/893b9cf4-5bb9-4257-9d19-baaea5438fd8)




![Screenshot 2025-04-22 121143](https://github.com/user-attachments/assets/a37ce821-446d-4c64-9b76-3ecd61b907f0)





