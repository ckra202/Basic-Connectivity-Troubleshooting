Basic-Connectivity-Troubleshooting
This repository is to showcase my ability to validate a system's network network stack using command line. 

# Network+ Lab 1 – Basic Connectivity Troubleshooting

# Objective
This lab simulates a real-world Tier 1 Help Desk scenario: a system that appears to be online but may have hidden network issues.  
The goal is to use basic command-line tools to validate local and external network connectivity.

# Tools Used
- Windows 10 Virtual Machine
- Command Prompt
- Basic Networking Commands (`ipconfig`, `ping`, `tracert`)

---

# Test Steps & Results

# `ipconfig /all`
Checked for:
- ✅ IP Address assigned correctly
- ✅ Subnet Mask and Default Gateway present
- ✅ DNS server configured
- ✅ DHCP enabled

# `ping 127.0.0.1`  
- ✅ Local loopback successful  
- Confirms that the network adapter and TCP/IP stack are functioning properly

# `ping <default gateway>`  
- ✅ Gateway reachable  
- Confirms local network connectivity to the router or default gateway

# `ping 8.8.8.8`  
- ✅ Google DNS server reachable by IP  
- Confirms external internet access without depending on DNS resolution

# `ping www.google.com`  
- ✅ DNS resolution successful  
- Confirms that the DNS server is working correctly and returning the proper IP address

# `tracert www.google.com`  
- ✅ Successful trace with multiple hops  
- Confirms that routing to external networks is functioning as expected

---

# What I Learned
- How to logically approach a layered network problem (Device → LAN → Internet → DNS)
- The difference between internal connectivity issues vs external routing problems
- The role of DNS in translating human-readable domains to IP addresses
- Practical use of troubleshooting commands used daily by support techs and SOC analysts

---

# Related Concepts
- Network+ Domain 1: Networking Concepts  
- OSI Layer 3 (Network) and Layer 7 (Application – DNS)  
- Help Desk ticket triage flow  
- Troubleshooting methodology (Layered approach: Physical → Logical)

---

# Repo Notes
This is part of my hands-on Network+ study series.  
All labs are designed to reinforce certification content through real-world application and analysis.
