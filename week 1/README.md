# SOC Fundamentals and Operations Lab

## Overview

This repository contains a comprehensive report on **Security Operations Center (SOC) Fundamentals**, covering core SOC concepts, security monitoring, log management, incident response, security tools, and practical hands-on labs using industry-standard technologies.

The project demonstrates how SOC teams monitor, detect, investigate, and respond to cybersecurity threats using SIEM platforms, log analysis, threat intelligence, and security monitoring workflows.

---

## Objectives

- Understand Security Operations Center (SOC) architecture and workflow.
- Learn SOC analyst roles and responsibilities.
- Perform security monitoring and log analysis.
- Build a basic SIEM environment using Elastic Stack.
- Detect and investigate security incidents.
- Configure alerting and dashboards.
- Gain practical experience with SOC tools and technologies.

---

## Topics Covered

### 1. SOC Fundamentals
- Purpose of a SOC
- Continuous Monitoring
- Threat Detection
- Incident Response
- Threat Intelligence Integration
- NIST Cybersecurity Framework (CSF)
- MITRE ATT&CK Framework

### 2. SOC Roles
- Tier 1 Analyst
- Tier 2 Analyst
- Tier 3 Analyst
- SOC Manager
- Threat Hunter

### 3. Security Monitoring
- Anomaly Detection
- Unauthorized Access Detection
- Policy Violation Monitoring
- Security Metrics
  - False Positives
  - False Negatives
  - Mean Time to Detect (MTTD)

### 4. Log Management
- Log Collection
- Log Normalization
- Log Storage
- Log Retention
- Log Analysis

### 5. Security Concepts
- CIA Triad
- Threat vs Vulnerability vs Risk
- Defense-in-Depth
- Zero Trust Security Model

### 6. Security Operations Workflow
- Detection
- Triage
- Investigation
- Response
- Recovery

### 7. Incident Response
- Preparation
- Identification
- Containment
- Eradication
- Recovery
- Lessons Learned

### 8. Documentation Standards
- Incident Reports
- Runbooks
- Standard Operating Procedures (SOPs)
- Post-Mortem Reports

---

## Practical Labs Performed

### Elastic Stack SOC Lab

Built a centralized logging and monitoring environment using:

- Elasticsearch
- Kibana
- Logstash
- Winlogbeat
- Ubuntu Linux
- Windows 11

### Architecture

```text
Windows Event Logs
        │
        ▼
   Winlogbeat
        │
        ▼
    Logstash
        │
        ▼
 Elasticsearch
        │
        ▼
     Kibana
```

### Activities

- Log Collection
- Log Normalization
- Security Monitoring
- Dashboard Creation
- KQL Query Practice
- Event Investigation

---

## Security Monitoring Exercises

### Failed Login Detection

Detected and analyzed:

- Windows Event ID 4625
- Multiple Failed Login Attempts
- Brute Force Indicators

### Network Traffic Analysis

Tools Used:

- Wireshark
- Kibana

Activities:

- SSH Traffic Monitoring
- Brute Force Detection
- Correlation of Network and Log Events

---

## Log Management Exercises

### Apache Log Normalization

Converted raw Apache access logs into structured JSON format using Logstash.

Extracted fields:

- Source IP
- HTTP Method
- URL
- Status Code
- Timestamp
- User Agent

---

## Security Tools Used

### SIEM

- Elasticsearch
- Kibana

### Log Processing

- Logstash
- Winlogbeat

### Network Analysis

- Wireshark

### IDS/IPS

- Snort

### Vulnerability Assessment

- Nessus

### Endpoint Monitoring

- Osquery

### Security Monitoring

- Wazuh

---

## Detection Engineering

### Elastic SIEM Alert Rule

Configured detection rules for:

- Failed Login Attempts
- Authentication Monitoring
- Brute Force Detection

### Wazuh Alerting

Implemented SSH brute-force detection using:

- Authentication Logs
- Built-in Wazuh Rules
- Custom Alert Logic

---

## Threat Hunting & Investigation

Activities included:

- IOC Analysis
- Event Correlation
- Log Investigation
- Browser History Analysis
- Security Event Documentation

Tools Used:

- BrowserHistoryView
- Windows Event Viewer
- Kibana
- Wazuh

---

## Key Learnings

- SOC operational workflow
- Log management lifecycle
- Security monitoring techniques
- SIEM implementation and management
- Threat detection and investigation
- Dashboard and visualization creation
- KQL querying
- Alert rule creation
- Incident response methodology
- IOC-based threat hunting

---

## Challenges Faced

- Kibana and Elasticsearch connectivity issues
- Log ingestion and timestamp formatting problems
- SSH service configuration issues
- KQL syntax troubleshooting
- Dashboard field mapping challenges
- Handling unstructured log data

---

## Technologies Used

| Category | Tools |
|-----------|--------|
| SIEM | Elasticsearch, Kibana |
| Log Collection | Winlogbeat |
| Log Processing | Logstash |
| Monitoring | Wazuh |
| Network Analysis | Wireshark |
| IDS/IPS | Snort |
| Vulnerability Scanning | Nessus |
| Endpoint Monitoring | Osquery |
| Operating Systems | Ubuntu, Windows 11 |

---

## References

- Elastic Stack Documentation
- Elasticsearch Documentation
- Kibana Documentation
- Wazuh Documentation
- MITRE ATT&CK Framework
- NIST SP 800-61
- Sigma Detection Rules
- Snort Documentation
- Osquery Documentation
- Microsoft Event ID Reference

---

## Author

**Akshay Kharat**

BCA Graduate | Cybersecurity Enthusiast | SOC Analyst Intern

---

## Disclaimer

This project was created for educational and learning purposes to demonstrate SOC concepts, SIEM implementation, security monitoring, and incident response workflows in a controlled lab environment.
