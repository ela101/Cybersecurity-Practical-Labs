# Lab - Packet Crafting with Scapy

## Objectives
In this lab, you will use Scapy, a Python-based packet manipulation tool, to craft custom packets. These custom packets will be used to perform reconnaissance on a target system.
-Use Scapy to Sniff Network Traffic.
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

## Create and Send a TCP SYN Packet
In this part, I will use Scapy to determine if port 445, a Microsoft Windows drive share port, is open on the target system at 10.6.6.23.

1. In the original Scapy terminal window, begin a packet capture on the internal interface attached to the 10.6.6.0/24 network. Use the interface name.
   >>> sniff(iface="br-internal")

2. Navigate to the second terminal window. Create and send a TCP SYN packet using the command shown.

   ![Tcp Sent](./tcp.png)

4. In the original Scapy terminal window, stop the packet capture by pressing CTRL-C. The output should be similar to that shown.

   ![Tcp Captured](./tcp_captured.png)

5. View the captured TCP packets using the nsummary() function. Display the detail of the TCP packet that was returned from the target computer at 10.6.6.23.
>>> a[packet number]

   ![View Packet](./view_packet.png)

