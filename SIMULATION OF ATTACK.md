###Here is the step-by-step workflow to simulate and detect the attack.
##phase 1:
You need to generate enough "noise" for the Intrusion Detection System (IDS) to pick it up. Standard pings might be ignored, so we will use more aggressive Nmap flags.
Identify the Target: Ensure your Security Onion "Management" or "Sniffing" interface IP is reachable.
Run an Aggressive Scan: Run the following command from your attacker machine:

###Command :sudo nmap -A -T4 -p- [Target_IP]
-A: Enables OS detection, version detection, script scanning, and traceroute (very noisy).
-T4: Speeds up the execution (more likely to trigger threshold alerts).
-p-: Scans all 65,535 ports.

<img width="597" height="175" alt="image" src="https://github.com/user-attachments/assets/8aea98d2-e62b-4b0e-98ea-33b0c089bf0f" />

##Phase 2: The Detection (Security Onion / Elasticsearch)
Once the scan finishes, Security Onion’s Suricata (the IDS engine) should have flagged the traffic.
Check the Alerts Dashboard
Log into your Security Onion Console (SOC).
Click on Alerts in the left-hand sidebar.
Look for signatures like:
GPL SCAN nmap fingerprint attempt
ET SCAN Potential SSH Scan
ET SCAN Nmap Scripting Engine User-Agent Detected

