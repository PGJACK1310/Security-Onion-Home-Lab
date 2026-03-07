# 🛡️ Security Onion Network Monitoring & Threat Detection Lab

- This project demonstrates network security monitoring and threat detection using Security Onion in a virtual lab environment. The system captures network traffic, analyzes suspicious activities using Suricata IDS and Zeek, and generates alerts for investigation through the Security Onion SOC dashboard.
---
# ✅ Project Overview

- Platform: Security Onion                                                                                                                                                                   
- Environment: Virtual Lab (VMware / VirtualBox)                                                                                                                                             
- Purpose: Simulate a SOC environment for monitoring and investigating security alerts                                                                                                       - Focus Areas:
- Network traffic monitoring
- Intrusion detection using Suricata
- Network analysis using Zeek
- Alert investigation using SOC dashboard
- Simulating cyber attacks for detection testing
---
# 🏗️ Lab Architecture
- This lab consists of three main components:
- Security Onion Server – Monitoring and detection platform
- Attacker Machine (Kali Linux) – Generates attack traffic
---
# 🚨 Simulated Attacks
- Two types of attacks were simulated to test detection capabilities.
- 🔎 1. Nmap Port Scanning Attack
- Attack command executed from attacker machine:
- sudo nmap -A -T4 -p- <TARGET_IP>
# Purpose of this attack:
- Scan all ports on the target system
- Identify open services
- Detect operating system and versions
- Generate suspicious traffic for IDS detection
---
# 🔐 2. SSH Brute Force Attack (Hydra)
- Password brute-force attack performed using Hydra.
Command used:
- hydra -l root -P passlist.txt -t 4 -V ssh://<TARGET_IP>
---
# 🧰 Tools & Technologies
| Tool                    | Purpose                              |
| ----------------------- | ------------------------------------ |
| **Security Onion**      | Network security monitoring platform |
| **Suricata**            | Intrusion Detection System (IDS)     |
| **Zeek**                | Network traffic analysis             |
| **Elastic Stack**       | Log collection and visualization     |
| **Wazuh**               | Host-based intrusion detection       |
| **VMware / VirtualBox** | Virtualization platform              |
| **Kali Linux**          | Attacker machine for simulations     |
---
