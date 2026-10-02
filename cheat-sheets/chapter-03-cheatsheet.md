## Chapter 3 Cheat Sheet — Entra Access Management & Identity Governance

### Conditional Access — 3 Components
| Component | What it does | Examples |
|---|---|---|
| Signals | Inputs evaluated | User/group, location, device platform/compliance, app, real-time risk |
| Decisions (Grant) | Outcome if conditions match | Block, require MFA, require compliant device, require approved app |
| Enforcement (Session) | Restricts in-session behavior | Limited browser access, app enforced restrictions, sign-in frequency |

**License:** Entra ID **P1**.

### Identity Protection — Risk Types
| Risk Type | Definition | Example Detections |
|---|---|---|
| Sign-in risk | Is this specific sign-in attempt suspicious? | Anonymous IP, impossible travel, malware-linked IP |
| User risk | Is this identity likely compromised? | Leaked credentials, unusual sign-in activity pattern |

**License:** Entra ID **P2**. Policies: require MFA on risk, block on high risk, force password change.

### PIM — Eligible vs Active
| State | Meaning |
|---|---|
| Eligible | Role inactive by default; user must activate (justification/MFA/approval); auto-expires |
| Active | Role permissions available immediately, no activation step |

**License:** Entra ID **P2**. Use for just-in-time admin access.

### Entra ID Governance Features
| Feature | Purpose |
|---|---|
| Access reviews | Recurring recertification of existing access (groups, apps, roles) with auto-removal |
| Entitlement management (access packages) | Bundle resources for self-service request + approval + expiration, ideal for guests/partners |

**License:** Entra ID Governance / P2.

### RBAC Basics
- Built-in roles: Global Administrator, User Administrator, Helpdesk Administrator, Application Administrator, etc.
- Principle of least privilege — assign narrowest role needed.
- Custom roles available for granular permission sets.

### Verified ID
- Decentralized identity based on **W3C Verifiable Credentials** standard.
- Issuer → Holder (user) → Verifier model.
- User controls and presents their own portable credential (e.g., proof of employment/education).

### Quick Decision Table
| Need | Use |
|---|---|
| Block sign-in unless MFA/compliant device | Conditional Access |
| Detect compromised accounts/sign-ins | Identity Protection |
| Time-bound admin role elevation | PIM |
| Bundle + self-service request access | Entitlement management |
| Periodic recheck of who still needs access | Access reviews |
| Portable, user-controlled digital credentials | Verified ID |

### Common Exam Traps
- Confusing sign-in risk (this attempt) with user risk (this identity).
- Thinking PIM = general access request tool (it's for privileged roles only).
- Assuming Conditional Access can bundle resources (it cannot — that's entitlement management).
- Forgetting license tiers: P1 = Conditional Access; P2 = Identity Protection, PIM, Governance features.
