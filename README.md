# cyart-soc-team

# SOC Alert-to-Response Capstone Project

## Overview

This repository contains practical SOC (Security Operations Center) learning activities, security monitoring exercises, incident response documentation, alert triage tasks, and a complete capstone project demonstrating the full alert-to-response lifecycle using Wazuh SIEM.

The project was performed in a controlled cybersecurity lab environment using Kali Linux, Metasploitable2, and Wazuh SIEM to simulate real-world attack detection and SOC investigation workflows.

---

# Objectives

* Understand SOC operations and workflows
* Learn SIEM-based security monitoring
* Perform log analysis and alert triage
* Simulate attacks in a lab environment
* Practice incident response procedures
* Implement evidence preservation techniques
* Map attacks using MITRE ATT&CK
* Create dashboards and security reports

---

# Lab Environment

| Component             | Purpose                               |
| --------------------- | ------------------------------------- |
| Kali Linux            | Attacker Machine                      |
| Metasploitable2       | Vulnerable Target Machine             |
| Wazuh SIEM            | Security Monitoring & Alert Detection |
| OpenSearch Dashboards | Visualization & Analysis              |
| Hydra                 | Brute-force Attack Simulation         |
| Wireshark             | Network Packet Analysis               |

---

# Project Structure

```text
SOC-Alert-to-Response-Capstone/
│
├── docs/
├── reports/
└── Screenshots/
```

---

# Topics Covered

## 1. SOC Fundamentals

* SOC roles and responsibilities
* Security monitoring concepts
* Threat detection workflow
* MITRE ATT&CK framework
* NIST incident response lifecycle

## 2. Security Monitoring

* SIEM monitoring using Wazuh
* Log collection and correlation
* Alert generation and prioritization
* Dashboard visualization

## 3. Log Management

* Syslog analysis
* Authentication log monitoring
* Failed login detection
* Log normalization concepts

## 4. Security Tools

* Wazuh SIEM
* Hydra
* Wireshark
* Snort
* Osquery
* Velociraptor

## 5. Incident Response

* Alert triage
* IOC analysis
* Containment planning
* Evidence preservation
* Documentation procedures

## 6. Capstone Project

* Simulated brute-force SSH attack using Hydra
* Detection through Wazuh SIEM
* Alert investigation and analysis
* MITRE ATT&CK mapping
* Incident documentation

---

# Capstone Project Workflow

```text
Attack Simulation
        ↓
Log Generation
        ↓
Wazuh SIEM Detection
        ↓
Alert Correlation
        ↓
Alert Triage
        ↓
Investigation
        ↓
Evidence Collection
        ↓
Documentation & Reporting
```

---

# Attack Simulation

The capstone project included a simulated brute-force SSH attack using Hydra against the Metasploitable2 virtual machine.

Example command used:

```bash
hydra -l msfadmin -P rockyou.txt ssh://192.168.1.x
```

The attack generated authentication failure logs which were detected and analyzed by Wazuh SIEM.

---

# MITRE ATT&CK Mapping

| Activity               | MITRE Technique |
| ---------------------- | --------------- |
| SSH Brute Force        | T1110           |
| Credential Access      | TA0006          |
| Initial Access Attempt | TA0001          |

---

# Key Learnings

* Security event monitoring using SIEM
* Alert classification and prioritization
* SOC investigation workflow
* Incident response lifecycle
* Threat intelligence integration
* Evidence preservation methods
* Security dashboard creation
* Practical cybersecurity operations

---

# Screenshots Included

* Wazuh Dashboard Alerts
* Hydra Attack Execution
* Alert Triage Screens
* Security Monitoring Dashboards
* Incident Response Documentation

---

# Skills Demonstrated

* SOC Operations
* SIEM Administration
* Log Analysis
* Alert Triage
* Threat Detection
* Incident Response
* MITRE ATT&CK Mapping
* Security Documentation
* Evidence Preservation

---

# References

* Wazuh Documentation
  https://documentation.wazuh.com

* MITRE ATT&CK Framework
  https://attack.mitre.org

* NIST SP 800-61 Incident Handling Guide
  https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final

* Hydra THC
  https://github.com/vanhauser-thc/thc-hydra

* OpenSearch Documentation
  https://opensearch.org/docs/latest/

* OWASP Logging Cheat Sheet
  https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html

---

# Disclaimer

This project was conducted in a controlled lab environment strictly for educational and defensive cybersecurity learning purposes. No unauthorized systems or networks were targeted.

---

# Author

Akshay Kharat
