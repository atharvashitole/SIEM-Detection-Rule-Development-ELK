# Credential Stuffing Detection Rule

## Overview

This detection rule identifies potential credential stuffing attacks by monitoring repeated failed authentication attempts. It searches for failed login events within the `training-logs` index and generates a high-severity alert whenever matching activity is detected.

---

## Rule Information

| Property | Value |
|----------|-------|
| Rule Name | Credential Stuffing Detection |
| Rule Type | Query Rule |
| Severity | High |
| Risk Score | 75 |
| Index Pattern | training-logs |
| Query Language | KQL |
| Runs Every | 1 Minute |
| Additional Look-back | 1 Minute |

---

## Detection Query

```kql
status : "failed"
```

---

## Detection Logic

The rule continuously monitors authentication logs stored in the `training-logs` index. Whenever a failed login event is detected, Elastic Security generates a high-severity alert for further investigation.

---

## Expected Output

- High-Severity Security Alert
- Failed Login Detection
- Rule Execution Recorded
- Alert Visible in Elastic Security Dashboard

---

## Skills Demonstrated

- SIEM Rule Development
- KQL Query Writing
- Elastic Security Detection Engineering
- Alert Validation
- Security Monitoring
