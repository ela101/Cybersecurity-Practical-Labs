# Lab - Packet Crafting with Scapy

## Objectives
In this lab, you will use Scapy, a Python-based packet manipulation tool, to craft custom packets. These custom packets will be used to perform reconnaissance on a target system.
-Investigate the Scapy Tool.
-Use Scapy to Sniff Network Traffic.
-Create and Send an ICMP Packet.
-Create and Send TCP SYN Packets.

## Use Scapy to Sniff Network Traffic
1. Launch Scapy sudo su scapy

   ![Scapy Launch](scapy.png)

2. Use the sniff() function to collect traffic using the default eth0 interface of my VM

   ![Sniff Function](sniff.png)

3. Open firefox browser and search an internet address lets take www.cisco.com

4. Return to the terminal window that is running the Scapy tool. Press CTRL-C to stop the capture. You should receive output which looks like to what is shown here:

   ![Captured Packet](./captured.png)
   
5. View the captured traffic as you did in Step 1d.
>>> a=_
>>> a.summary()

   ![Packets Read](./packets.png)

## Create and Send an ICMP Packet

