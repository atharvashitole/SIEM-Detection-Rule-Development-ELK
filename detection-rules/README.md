# Detection Rules

## Overview

This folder contains the custom SIEM detection rules developed as part of the **SIEM Detection Rule Development using the Elastic (ELK) Stack** project.

The rules were created and tested in **Elastic Security** to detect common cyber attack techniques by monitoring security events and generating alerts for further investigation.

---

## Detection Rules Included

### Credential Stuffing Detection

Detects repeated failed authentication attempts that may indicate credential stuffing or password guessing attacks.

**Index:** `training-logs`

---

### DNS Tunnelling Detection

Detects suspicious DNS queries associated with potential DNS tunnelling and covert communication.

**Index:** `dns-logs`

---

### PowerShell Exploitation Detection

Detects suspicious PowerShell command-line activity commonly used during malicious execution and post-exploitation.

**Index:** `powershell-logs`

---

## Detection Features

- Custom KQL detection queries
- High-severity alert generation
- Scheduled rule execution
- Alert validation in Elastic Security
- Detection engineering using the Elastic (ELK) Stack

---

## Purpose

These detection rules demonstrate practical SIEM implementation, security monitoring, and detection engineering skills using Elastic Security. They were developed, tested, and validated as part of a hands-on cybersecurity internship project.
