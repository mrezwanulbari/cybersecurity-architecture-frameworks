# NIST Cybersecurity Framework (CSF) Governance Mapping

Maps the NIST CSF core functions to governance artifacts and architecture decisions, for teams building a compliance-mapped architecture rather than architecture and compliance as separate, disconnected workstreams.

| CSF Function | Architecture Touchpoint | Typical Evidence |
|---|---|---|
| **Identify** | Asset inventory feeding entity/CMDB systems, risk assessment scope | Asset inventory reports, risk register |
| **Protect** | Identity layer, network segmentation, data encryption controls | IAM policies, network diagrams, encryption standards docs |
| **Detect** | SIEM/SOAR detection coverage, EDR deployment | Detection rule library, coverage-to-ATT&CK mapping |
| **Respond** | Incident response playbooks, SOAR automation | IR playbooks, tabletop exercise records |
| **Recover** | Backup/DR architecture, recovery testing | Backup test results, RTO/RPO documentation |

## Why Map Architecture to CSF Explicitly

Architecture decisions made without an explicit compliance mapping tend to satisfy the compliance requirement accidentally or not at all — teams find out during an audit which controls actually count as evidence, rather than designing with the mapping in mind from the start. Building the mapping into the architecture documentation from day one turns audit prep from a scramble into a report-generation exercise.

---
*Part of the [cybersecurity-architecture-frameworks](../README.md) repository.*
