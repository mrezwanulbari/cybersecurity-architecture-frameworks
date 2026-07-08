# Security Monitoring Architecture

Defines how logs, alerts, detections, and telemetry flow into the SOC.

## Monitoring Layers

### 1. Endpoint Telemetry
- EDR/XDR  
- Process creation  
- Network connections  

### 2. Identity Telemetry
- Authentication logs  
- Conditional Access events  
- Privilege escalation  

### 3. Cloud Telemetry
- Azure Activity Logs  
- AWS CloudTrail  
- CSPM findings  

### 4. Network Telemetry
- Firewall logs  
- DNS logs  
- Proxy logs  

## SIEM Integration
- Normalization  
- Enrichment  
- Correlation  
- MITRE mapping  

## MITRE Alignment
- T1059 (Execution)  
- T1021 (Remote Services)
