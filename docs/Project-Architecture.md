# Project Architecture

## Overview

This project demonstrates the implementation of a Security Information and Event Management (SIEM) solution using the Elastic (ELK) Stack. The environment was configured to collect security logs, process events, detect suspicious activities, and generate alerts using Elastic Security.

---

## Architecture Components

### Elasticsearch

Elasticsearch serves as the central data store for security events. It indexes log data and enables fast searching and analysis of security information.

### Logstash

Logstash processes incoming log data, applies parsing and transformations where required, and forwards the events to Elasticsearch.

### Kibana

Kibana provides visualization, monitoring, and investigation capabilities. It was used to configure detection rules, investigate alerts, and validate detection results.

### Elastic Security

Elastic Security was used to create and manage custom detection rules for identifying simulated cyber attack techniques.

---

## Data Flow

```
Sample Logs
      │
      ▼
 Logstash
      │
      ▼
 Elasticsearch
      │
      ▼
 Elastic Security
      │
      ▼
 Security Alerts
      │
      ▼
 Investigation using Kibana
```

---

## Detection Workflow

1. Sample security logs were generated.
2. Log events were indexed into Elasticsearch.
3. Custom detection rules were created in Elastic Security.
4. Detection rules continuously monitored indexed events.
5. Matching events generated security alerts.
6. Alerts were investigated and validated using Kibana.

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

## Outcome

The implemented architecture successfully detected simulated Credential Stuffing, DNS Tunnelling, and PowerShell Exploitation activities using custom SIEM detection rules.
