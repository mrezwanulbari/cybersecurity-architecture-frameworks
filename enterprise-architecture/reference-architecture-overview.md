# Enterprise Reference Architecture Overview

A layered reference architecture for enterprise security programs, showing how the major domains (identity, network, endpoint, data, cloud) fit together rather than being designed in isolation.

## Layered Model

1. **Governance Layer** — policy, risk management, compliance mapping (ISO 27001, NIST CSF). Everything below should trace back to a governance requirement, not exist as a standalone tool purchase.
2. **Identity Layer** — the foundation layer in a Zero Trust model. IAM, PAM, MFA, conditional access. Every other layer's access decisions ultimately depend on identity layer integrity.
3. **Network Layer** — segmentation, ZTNA, encrypted transport. Assumes identity layer signals feed network access decisions (not static network-location-based trust).
4. **Endpoint Layer** — EDR, device compliance posture, patch management. Feeds device-trust signals up to the network and application layers.
5. **Application/Workload Layer** — secure SDLC, API security, secrets management, workload identity for service-to-service auth.
6. **Data Layer** — classification, encryption, DLP. The layer everything else ultimately exists to protect.

## Design Principle: Signal Flow, Not Just Tool Stack

The common failure mode in enterprise architecture is deploying strong tools at each layer that don't share signal with each other — an EDR that detects device compromise but doesn't feed that signal into the network access control layer, so a compromised device retains full network access until a human manually intervenes. The architecture value is in the *connective tissue* between layers, not just the individual tool capability.

## Cloud Architecture Considerations

See [aws-security](https://github.com/mrezwanulbari/aws-security) and [azure-security](https://github.com/mrezwanulbari/azure-security) for cloud-specific implementations of this layered model — the layers stay the same, but identity layer shifts toward cloud IAM/federation and network layer shifts toward cloud-native segmentation (security groups, NSGs, VPC/VNet design).

---
*Part of the [cybersecurity-architecture-frameworks](../README.md) repository.*
