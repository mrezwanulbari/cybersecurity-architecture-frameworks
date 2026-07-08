# Data Protection Architecture

Protecting sensitive data requires encryption, classification, access control, and monitoring.

## Data Protection Layers

### 1. Classification
- Public  
- Internal  
- Confidential  
- Restricted  

### 2. Encryption
- At rest (AES-256)  
- In transit (TLS 1.2+)  
- Key management (HSM, KMS)  

### 3. Access Control
- Attribute-based access control (ABAC)  
- Data loss prevention (DLP)  
- Tokenization for sensitive fields  

### 4. Monitoring
- Data access logs  
- Anomaly detection  
- Insider threat analytics  

## MITRE Alignment
- T1005 (Data from Local System)  
- T1530 (Data from Cloud Storage)
