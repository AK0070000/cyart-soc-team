 SOC Operations and Cybersecurity Lab Project

## Overview

This repository contains a complete hands-on cybersecurity and SOC (Security Operations Center) lab project performed in a virtual environment using various offensive and defensive security tools. The project covers secure network design, penetration testing, SIEM monitoring, threat intelligence integration, traffic analysis, incident response, evidence collection, and SOC workflow simulation.

The objective of this project was to gain practical exposure to real-world SOC operations, network security monitoring, attack detection, incident escalation, and response workflows using industry-relevant tools and techniques.

---

# Project Modules

## 1. Secure Network Design

Designed a secure enterprise-style network topology including:

* DMZ (Demilitarized Zone)
* VLAN segmentation
* Firewall placement
* IDS/IPS integration
* Proxy server
* Internal employee network
* Guest network
* Web and database servers

### Security Concepts Covered

* Network segmentation
* Defense-in-depth
* Attack surface reduction
* Access control
* Traffic isolation
* Secure architecture planning

### Tools Used

* draw.io
* VirtualBox Networking

---

# 2. Penetration Testing with Metasploit

Performed vulnerability scanning and exploitation against Metasploitable2.

### Activities Performed

* Nmap scanning
* Service enumeration
* Vulnerability identification
* Exploitation using Metasploit Framework

### Exploits Used

## vsFTPd 2.3.4 Backdoor Exploit

```bash
use exploit/unix/ftp/vsftpd_234_backdoor
```

## UnrealIRCd Backdoor Exploit

```bash
use exploit/unix/irc/unreal_ircd_3281_backdoor
```

### Key Learnings

* Mapping services to vulnerabilities
* Understanding exploit selection
* Remote shell access
* Post-exploitation basics
* Importance of patch management

### Tools Used

* Metasploit Framework
* Nmap
* Kali Linux
* Metasploitable2

---

# 3. Wireshark Traffic Analysis

Captured and analyzed network traffic using Wireshark.

### Protocols Analyzed

* TCP
* UDP
* ICMP
* TLS/HTTPS
* ARP

### Traffic Patterns Studied

* SYN packets
* SYN-ACK responses
* ACK packets
* FIN-ACK termination
* TLS Client Hello
* HTTPS encrypted traffic behavior

### Key Learnings

* TCP three-way handshake
* Connection termination process
* Encrypted traffic metadata analysis
* Packet flow analysis
* Network behavior monitoring

### Tools Used

* Wireshark
* Kali Linux

---

# 4. Python-Based Packet Analysis

Developed custom Python scripts for network packet analysis.

### Features Implemented

* Packet sniffing
* Protocol counting
* Traffic categorization
* Packet logging
* Visualization using graphs
* Report generation

### Libraries Used

```python
scapy
matplotlib
collections
datetime
```

### Output Generated

* Packet reports
* Protocol distribution charts
* Traffic summaries

---

# 5. SIEM Monitoring and Log Analysis

Configured and worked with SIEM technologies for security monitoring.

### Activities Performed

* Log collection
* Log correlation
* Event analysis
* Alert monitoring
* Dashboard visualization

### Concepts Covered

* Event ID analysis
* Failed login detection
* Anomaly detection
* Threat detection workflows
* SOC monitoring lifecycle

### Tools Used

* Wazuh
* Elastic Stack
* Kibana

---

# 6. Threat Intelligence Integration

Integrated threat intelligence into the SOC workflow.

### Activities Performed

* AlienVault OTX feed integration
* IOC matching
* Alert enrichment
* Threat hunting
* Reputation checking

### MITRE ATT&CK Techniques Studied

* T1078 – Valid Accounts
* T1110 – Brute Force
* T1210 – Exploitation of Remote Services

### Tools Used

* Wazuh
* AlienVault OTX
* VirusTotal

---

# 7. Incident Escalation and SOC Workflow

Simulated SOC incident handling and escalation procedures.

### Activities Performed

* Alert triage
* Case creation
* Incident escalation
* SITREP drafting
* Tier 1 to Tier 2 escalation workflow
* Mock SOAR playbook creation

### Concepts Covered

* SOC escalation tiers
* Incident response lifecycle
* Threat communication
* Incident documentation

### Tools Used

* TheHive
* Google Docs
* Splunk Phantom (mock workflow)

---

# 8. Evidence Preservation and Digital Forensics

Performed basic evidence collection and preservation.

### Activities Performed

* Network connection collection
* Memory dump acquisition
* SHA256 hashing
* Chain-of-custody documentation

### Tools Used

* FTK Imager
* Windows Commands
* SHA256 hashing utilities

---

# 9. CrowdSec Containment Simulation

Configured CrowdSec for attack containment simulation.

### Activities Performed

* CrowdSec installation
* Decision engine testing
* IP banning simulation
* Manual firewall blocking using iptables

### Key Concepts Learned

* Threat containment
* Automated banning
* Decision engine workflow
* Firewall enforcement

### Tools Used

* CrowdSec
* iptables

---

# 10. Full SOC Capstone Simulation

Performed a complete SOC workflow simulation from attack to reporting.

### Workflow Covered

1. Attack Simulation
2. Detection
3. Alert Triage
4. Threat Intelligence Validation
5. Containment
6. Escalation
7. Reporting
8. Management Briefing

### Skills Demonstrated

* Penetration testing
* SOC monitoring
* Threat hunting
* Incident response
* Documentation
* Security analysis

---

# Technologies and Tools Used

| Category            | Tools                                |
| ------------------- | ------------------------------------ |
| Penetration Testing | Metasploit, Nmap                     |
| Traffic Analysis    | Wireshark, Scapy                     |
| SIEM                | Wazuh, Elastic, Kibana               |
| Threat Intelligence | AlienVault OTX, VirusTotal           |
| Incident Response   | TheHive                              |
| Forensics           | FTK Imager                           |
| Containment         | CrowdSec, iptables                   |
| Visualization       | Matplotlib, draw.io                  |
| Operating Systems   | Kali Linux, Windows, Metasploitable2 |

---

# Key Skills Gained

* SOC Operations
* Threat Detection
* Incident Response
* Penetration Testing
* Traffic Analysis
* Threat Hunting
* SIEM Monitoring
* Log Correlation
* Network Security
* Digital Forensics
* Threat Intelligence Integration
* Security Documentation

---

# Challenges Faced

* Elasticsearch service failures
* Wazuh configuration issues
* CrowdSec firewall bouncer limitations
* TheHive installation problems
* DNS and repository issues in Kali Linux
* Log parsing and rule tuning
* False positives in IDS alerts

---

# Conclusion

This project provided practical exposure to real-world SOC workflows, penetration testing, network monitoring, incident escalation, and threat intelligence operations. The hands-on activities helped in understanding how offensive and defensive cybersecurity operations work together in enterprise environments. It also improved troubleshooting, analytical, and incident response skills through practical implementation and simulated attack scenarios.

---

# Repository Structure

```bash
/project-folder
│
├── reports/
├── screenshots/
├── scripts/
├── diagrams/
├── logs/
├── traffic-analysis/
├── metasploit-results/
├── wazuh-rules/
├── crowdsec/
└── README.md
```

---

# Author

## Akshay Kharat

BCA Student | Cybersecurity Enthusiast | SOC & Penetration Testing Learner

---

# Disclaimer

This project was performed in a controlled lab environment for educational and research purposes only. Do not use these techniques on unauthorized systems or networks.
