# Network Segmentation Architecture

Network segmentation reduces lateral movement risk by isolating critical assets, enforcing least privilege, and creating defensible boundaries.

## Segmentation Model

### 1. Tier-Based Segmentation
- Tier 0: Domain controllers, identity systems  
- Tier 1: Application servers  
- Tier 2: User workstations  
- Tier 3: External-facing systems  

### 2. Micro-Segmentation
- Enforce workload-to-workload policies  
- Use identity-based segmentation (AAD, workload identities)  
- Apply Zero Trust principles  

### 3. East-West Traffic Monitoring
- Deploy sensors in internal VLANs  
- Use behavioral analytics for lateral movement detection  

## Controls
- Firewall policies  
- NAC enforcement  
- Conditional Access  
- EDR/XDR network telemetry  

## MITRE Alignment
- T1021 (Remote Services)  
- T1078 (Valid Accounts)  
- T1046 (Network Scanning)
