## Chapter 8 Cheat Sheet: Purview Records, Insider Risk, eDiscovery, Privacy

### Retention: Policy vs Label
| Feature | Retention Policy | Retention Label |
|---|---|---|
| Scope | Container (site, mailbox, all locations) | Item-level |
| Applied by | Admin, bulk | Admin (manual/auto) or user |
| Travels with content | No | Yes |
| Records declaration | No | Yes (Record / Regulatory Record) |
| Auto-apply triggers | N/A | Sensitive info types, trainable classifiers, keywords |

**Conflict resolution order:** 1) Retention beats deletion → 2) Longest retention wins → 3) Explicit label beats implicit policy.

**Record vs Regulatory Record:** Record blocks edit/delete but admin can remove label. Regulatory Record blocks even label removal until retention expires — strictest option.

### eDiscovery Tiers
| Tool | Case Mgmt | Holds | Review Sets | Analytics | Custodians | License |
|---|---|---|---|---|---|---|
| Content Search | No | No | No | No | No | Any |
| eDiscovery Standard | Yes | Yes | No | No | No | E3 |
| eDiscovery Premium | Yes | Yes | Yes | Near-dup, email threading | Yes | E5/add-on |

### Audit
| Tier | Default Retention | Extended Retention | Crucial Events | License |
|---|---|---|---|---|
| Standard | 180 days | No | No | E1/E3 |
| Premium | 365 days | 1/7/10 yr add-on | Yes (e.g. MailItemsAccessed) | E5 |

### Insider Risk Management
- **Purpose:** ML-based detection of risky insider activity (theft, leaks, sabotage) with pseudonymized identities for privacy.
- **License:** M365 E5 or Insider Risk Management add-on.
- **Templates:** Data theft by departing users, Data leaks, Data leaks (priority users), Patent/confidential info leaks, Security policy violations, General.

### Communication Compliance
- Detects inappropriate/risky message content (harassment, threats, sensitive data, regulatory violations).
- Sources: Teams, Exchange, Yammer, third-party connectors.
- License: E5/add-on. Distinct from Insider Risk (behavior/exfiltration) and DLP (data type match).

### Microsoft Service Trust Portal
- Repository of audit reports (SOC 1/2/3), ISO 27001/27018 certifications, trust documents.
- Read-only reference resource — not for configuring tenant compliance settings (that's the Purview compliance portal / Compliance Manager).

### Microsoft Privacy Principles
- **Control** — customer owns/manages their data.
- **Transparency** — clear about collection/use of data.
- **Security** — strong protection via encryption and access control.
- Also: Strong legal protections, No content-based ad targeting, Benefits to the customer.

### Exam Gotchas
- Retention **always** beats deletion in conflicts.
- eDiscovery Standard has NO review sets or analytics — that's Premium only.
- Audit Standard = 180 days; Audit Premium = 365 days default (extendable).
- Service Trust Portal ≠ Compliance Manager (reports vs action-tracking tool).
