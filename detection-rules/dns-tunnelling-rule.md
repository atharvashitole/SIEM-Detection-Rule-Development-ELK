# DNS Tunnelling Detection Rule

## Overview

This detection rule identifies potential DNS tunnelling activity by monitoring DNS queries that contain suspicious domains. It searches DNS events stored in the `dns-logs` index and generates a high-severity alert whenever matching traffic is detected.

---

## Rule Information

| Property | Value |
|----------|-------|
| Rule Name | DNS Tunnelling Detection |
| Rule Type | Query Rule |
| Severity | High |
| Risk Score | 75 |
| Index Pattern | dns-logs |
| Query Language | KQL |
| Runs Every | 1 Minute |
| Additional Look-back | 1 Minute |

---

## Detection Query

```kql
query : "*attacker.com"
```

---

## Detection Logic

The rule continuously monitors DNS query logs stored in the `dns-logs` index. Whenever a DNS request containing the configured suspicious domain is detected, Elastic Security generates a high-severity alert for further investigation.

---

## Expected Output

- High-Severity Security Alert
- Suspicious DNS Query Detection
- Rule Execution Recorded
- Alert Visible in Elastic Security Dashboard

---

## Skills Demonstrated

- SIEM Rule Development
- KQL Query Writing
- DNS Traffic Monitoring
- Elastic Security Detection Engineering
- Threat Detection and Alert Validation
