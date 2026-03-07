🛡️ Security Onion Network Security Monitoring Lab

📌 Project Overview                                                                                                                                                                       
This project demonstrates the deployment and configuration of Security Onion, a powerful open-source platform used for Network Security Monitoring (NSM), Intrusion Detection, and Threat Analysis.                                                                                                                                                                                
The lab environment simulates real-world cyber attacks such as port scanning and brute-force attacks, and shows how Security Onion detects and analyzes these threats using tools like Suricata, Zeek, Elastic Stack                                                                                                                                                             

🎯 Project Objectives                                                                                                                                                                     
Deploy Security Onion in a virtual lab environment                                                                                                                                        
Configure network monitoring and intrusion detection                                                                                                                                      
Simulate cyber attacks from an attacker machine                                                                                                                                           
Detect malicious activity using Suricata IDS and Zeek                                                                                                                                     
Analyze logs and alerts through Elastic dashboards                                                                                                                                        
Investigate incidents using the Security Onion SOC console                                                                                                                                

🧰 Tools & Technologies
| Tool                    | Purpose                              |
| ----------------------- | ------------------------------------ |
| **Security Onion**      | Network security monitoring platform |
| **Suricata**            | Intrusion Detection System (IDS)     |
| **Zeek**                | Network traffic analysis             |
| **Elastic Stack**       | Log collection and visualization     |
| **VMware / VirtualBox** | Virtualization platform              |
| **Kali Linux**          | Attacker machine for simulations     |

🏗️ Lab Architecture                                                                                                                                                                      

The lab environment consists of the following components:
Attacker Machine (Kali Linux)                                                                                                                                                             
        │
        │ Attack Traffic
        ▼
   Target Network
        │
        ▼
Security Onion Sensor
        │
        ▼
SOC Dashboard (Elastic + Kibana)

📊 Results                                                                                                                                                                                
The system successfully detected simulated attacks and displayed them in the SOC dashboard.
Detected activities included:
Port scanning
SSH brute-force attempts
Suspicious network traffic
Security Onion provided detailed logs and alerts for investigation.
