# Chapter 4 Cheat Sheet: Azure Infrastructure Security & Defender for Cloud

## Network Security Service Selection
| Service | OSI Layer | Purpose | Cost |
|---|---|---|---|
| NSG | 3/4 | Allow/deny by IP, port, protocol; stateful; applied to subnet/NIC | Free |
| Azure Firewall | 3–7 | Centralized managed firewall; FQDN filtering; threat intelligence; cross-VNet/subscription policy via Firewall Manager | Paid |
| WAF | 7 (HTTP/S only) | Blocks OWASP Top 10 (SQLi, XSS); deployed on App Gateway, Front Door, CDN | Paid |
| Azure Bastion | N/A (access) | Secure browser-based RDP/SSH without public IP on VM | Paid |

**Rule of thumb:** Web app exploit → WAF. Subnet-level IP/port filtering → NSG. Centralized outbound/FQDN control → Azure Firewall. Secure remote VM access → Bastion.

## Azure DDoS Protection Tiers
| Tier | Cost | SLA | Cost Protection | Rapid Response |
|---|---|---|---|---|
| Basic | Free, automatic | No | No | No |
| IP Protection | Paid (per public IP) | Yes | Limited | Limited |
| Network Protection (Standard) | Paid | Yes | Yes | Yes |

**Exam trigger words:** "SLA guarantee", "cost protection", "Rapid Response team" → Network Protection.

## Azure Bastion Requirements
- Subnet name: `AzureBastionSubnet` (exact, case-sensitive)
- Minimum subnet size: `/26`
- Access via Azure portal over TLS 443 — no public IP needed on target VM

## Microsoft Defender for Cloud
- **CSPM (Cloud Security Posture Management):** continuous config assessment; Foundational CSPM = free; Defender CSPM plan = paid (adds attack path analysis, agentless scanning)
- **CWP (Cloud Workload Protection):** runtime threat protection for VMs, containers, SQL, storage, etc. (paid Defender plans per resource type)
- **Secure Score:** % = completed recommendation points ÷ total possible points. Enabling a plan ≠ score increase; remediating recommendations does.
- **Regulatory Compliance Dashboard:** maps recommendations to standards (PCI-DSS, ISO 27001, SOC 2, NIST) using Microsoft Cloud Security Benchmark (MCSB) as default baseline.

## Network Segmentation
- Hub-spoke topology: central hub (firewall, gateway) + isolated spoke VNets for workloads
- Limits lateral movement; enforced via NSGs, Azure Firewall, and UDRs (user-defined routes)

## Common Exam Traps
- Confusing NSG (free, L3/4) with Azure Firewall (paid, L3-7, FQDN)
- Assuming DDoS Basic includes cost protection/SLA — it does not
- Forgetting Bastion subnet name/size requirements
- Believing enabling a Defender plan alone raises secure score
