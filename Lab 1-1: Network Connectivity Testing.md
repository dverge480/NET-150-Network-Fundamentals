# Lab 1-1: Network Connectivity Testing

This lab aims to explore network connectivity and diagnostic tools, using commands like ipconfig, ping, tracert, and nslookup to analyze local and internet networks, gather system information, and test communication.

### Objectives: 
- Turn your firewall off so others can "ping" your system
- Discover network information about your system using the command line tool ipconfig
- Test network connectivity to other systems in our Local Network using the command ping
- Test network connectivity to the Internet by "pinging" a Google server

#### VM connection type must be set to Bridged.


Turn off Windows Defender Firewall for both public and private areas
Run ipconfig and record the default gateway, IPv4 address, and subnet mask
Run ipconfig /all and record the MAC address and any DNS Servers.
Ping the default gateway recorded in step 2
Now ping www.google.com

#### How are the results different from pinging a website compared to a local ip of another computer?
When pinging a website, a public IP address is recognized in contrast to the private IP address recognized when pinging a local computer. Also, pinging a local computer or something on the same LAN does not always require a DNS resolution, while pinging a website does.
