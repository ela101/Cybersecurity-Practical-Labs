# Nmap Practical Lab Documentation
This folder contains all Nmap scans replicated from the classroom practical session, including screenshots, summaries, and explanations of each command.

1. Host Discovery Scan Command: nmap -sn 10.6.6.0/24 Purpose: Performs a ping sweep to identify active hosts in the subnet.
   Screenshot:

![Host Discovery Scan](./host-discovery.png)

2. OS Fingerprinting Command: sudo nmap -O 10.6.6.23 Purpose: Identifies operating system using stack fingerprinting.
   screenshot:

![OS Discovery Scan](./os-discovery.png)

3. Service Detection + Aggressive Scan Command: nmap -p21 -sV -A -T4 10.6.6.23 Purpose: Detects services, versions, OS, traceroute, and runs scripts.
   screenshot:

![Service Aggressive Scan](./service_aggresive.png)

4. 



