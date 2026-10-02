## Chapter 1 Cheat Sheet: Security, Compliance & Identity Foundations

### Shared Responsibility Model
| Layer | On-Prem | IaaS | PaaS | SaaS |
|---|---|---|---|---|
| Data & Identities | Customer | Customer | Customer | Customer |
| Applications | Customer | Customer | Customer | Provider |
| OS Patching | Customer | Customer | Provider | Provider |
| Network Controls | Customer | Shared | Provider | Provider |
| Physical Hosts/Datacenter | Customer | Provider | Provider | Provider |

**Rule:** Data, identity, endpoints, and access management NEVER shift to the provider — in any model.

### Zero Trust — 3 Guiding Principles (VLA)
1. **Verify explicitly** — auth on all signals (identity, device, location, data sensitivity)
2. **Least privilege access** — JIT/JEA, risk-based policies
3. **Assume breach** — segment, encrypt, monitor as if attacker is already inside

### Defense in Depth (outer → inner)
Physical → Identity & Access → Perimeter → Network → Compute → Application → **Data (center)**

### Authentication vs. Authorization
| Concept | Question Answered | Example |
|---|---|---|
| Authentication | Who are you? | Username + password, MFA |
| Authorization | What can you do? | Role/group membership, RBAC |

**Order matters:** Authenticate → then Authorize.

### Encryption vs. Hashing
| Concept | Reversible? | Purpose |
|---|---|---|
| Encryption | Yes (with key) | Confidentiality |
| Hashing | No (one-way) | Integrity, password storage |

### Common Threat Types
| Threat | Goal | Mechanism |
|---|---|---|
| Phishing | Steal credentials/info | Deceptive email/link, social engineering |
| Ransomware | Extort payment | Encrypts victim data |
| DDoS | Disrupt availability | Flood service with traffic from many sources |

### GRC Basics
- **Governance:** policies, oversight, accountability
- **Risk:** identify, assess, mitigate threats to objectives
- **Compliance:** meet legal/regulatory/contractual obligations
- GRC is a **framework/discipline**, not a specific product.

### Exam Traps
- Confusing authentication (identity proof) with authorization (permission check)
- Thinking hashing can be reversed like encryption
- Assuming DDoS steals data (it disrupts availability only)
- Believing the provider ever owns customer data/identity responsibility
- Forgetting Zero Trust applies to INTERNAL users too, not just external
