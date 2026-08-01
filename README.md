<p align="center">
  <img src="assetbanner.png" alt="SIEM Detection Rule Development Banner" width="100%">
</p>

# SIEM Detection Rule Development using Elastic (ELK) Stack

## Overview

This project demonstrates the implementation and testing of custom SIEM correlation rules using the Elastic (ELK) Stack. The objective was to simulate common cyber attack techniques, generate security events, and validate custom detection rules in Elastic Security.

The project covers three attack scenarios:

- Credential Stuffing Detection
- DNS Tunnelling Detection
- PowerShell Exploitation Detection

---

## Objectives

- Deploy and configure the Elastic (ELK) Stack.
- Create custom SIEM detection rules.
- Simulate attack scenarios.
- Generate security alerts.
- Validate detection rule effectiveness.
- Investigate alerts using Elastic Security.

---

## Technologies Used

- Elasticsearch
- Kibana
- Logstash
- Elastic Security
- Docker
- Windows
- KQL (Kibana Query Language)

---

## Detection Rules Implemented

### Credential Stuffing Detection

Detects repeated failed authentication attempts that may indicate password guessing or credential stuffing attacks.

### DNS Tunnelling Detection

Detects suspicious DNS queries that may indicate data exfiltration or covert communication.

### PowerShell Exploitation Detection

Detects suspicious PowerShell commands such as:

- EncodedCommand
- ExecutionPolicy Bypass
- Invoke-WebRequest

---

## Project Structure

```
SIEM-Detection-Rule-Development-ELK
│
├── docs/
├── detection-rules/
├── report/
├── screenshots/
└── README.md
```

---

## Results

Successfully developed and validated custom SIEM detection rules.

The implemented rules generated security alerts for:

- Credential Stuffing
- DNS Tunnelling
- PowerShell Exploitation

The generated alerts were investigated using the Elastic Security dashboard to confirm successful detection.

---

## Skills Demonstrated

- SIEM Engineering
- Detection Engineering
- Security Monitoring
- Elastic Security
- ELK Stack Administration
- Incident Detection
- Security Alert Investigation

---

## Author

**Atharva Shitole**

Cybersecurity Graduate
