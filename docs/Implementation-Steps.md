# Implementation Steps

## Overview

This document describes the implementation process followed to develop and validate custom SIEM detection rules using the Elastic (ELK) Stack.

---

## Step 1 – Environment Setup

- Installed Docker Desktop.
- Deployed Elasticsearch, Kibana, and Logstash using Docker Compose.
- Verified that all services were running successfully.
- Confirmed access to Kibana through the web interface.

---

## Step 2 – Log Ingestion

- Created sample log indices for different attack scenarios.
- Inserted simulated security events into Elasticsearch.
- Verified successful indexing using Kibana Dev Tools.

---

## Step 3 – Detection Rule Development

Three custom detection rules were created in Elastic Security:

### Credential Stuffing Detection

A query rule was configured to detect repeated failed authentication attempts from the `training-logs` index.

### DNS Tunnelling Detection

A query rule was created to identify suspicious DNS queries associated with DNS tunnelling activity from the `dns-logs` index.

### PowerShell Exploitation Detection

A query rule was developed to detect suspicious PowerShell command-line activity from the `powershell-logs` index.

---

## Step 4 – Alert Generation

- Sample attack events were generated.
- Detection rules were executed automatically.
- Elastic Security successfully generated alerts for each simulated attack.

---

## Step 5 – Testing and Validation

The generated alerts were reviewed and validated using the Elastic Security dashboard.

Testing confirmed that all implemented detection rules successfully identified the simulated attack scenarios.

---

## Outcome

The project successfully demonstrated the implementation, testing, and validation of custom SIEM detection rules using the Elastic (ELK) Stack. The completed environment provided practical experience in security monitoring, detection engineering, and alert investigation.
