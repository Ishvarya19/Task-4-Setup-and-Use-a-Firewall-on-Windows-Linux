# Task 4 – Firewall Configuration Report

# Objective
Configure and test basic firewall rules to allow or block network traffic on a system.

# Tools Used
- **Windows Firewall** (GUI & PowerShell)
- **UFW** (Uncomplicated Firewall) on Linux

# Steps Performed 
1. Open Windows Firewall tool   
   Press `Windows + R`, type `wf.msc`, and press Enter.
2. View Current Rules 
   Navigated to Inbound Rules and * Outbound Rules *.
3. Block Port 23 (Telnet)  
   - New Rule → Port → TCP → 23 → Block connection.
4. Test the Rule
   - `telnet localhost 23`
   Results: Connection blocked.
5. Remove Test Rule
   Deleted the Telnet block rule after testing.

# Steps Performed Linux UFW
- sudo ufw enable
- sudo ufw status numbered
- sudo ufw deny 23/tcp
- sudo ufw allow 22/tcp
- sudo ufw delete deny 23/tcp

# Summary – How Firewall Filters Traffic
A firewall monitors and controls incoming and outgoing network traffic based on pre-defined rules.
It can:

1. Allow safe traffic
2. Block risky or unauthorized traffic

Rules can be:

1. Inbound (coming to the system)
2. Outbound (leaving the system)

# Outcome
Successfully configured and tested firewall rules, understood inbound/outbound filtering, and gained hands-on experience with Windows Firewall and UFW on Linux.

If you want, I can now also give you **matching `.txt` and `.pdf` versions** of this so your GitHub repo looks complete like your previous tasks. Do you want me to prepare those files?
