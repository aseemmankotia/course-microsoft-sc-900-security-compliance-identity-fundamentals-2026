## Chapter 7 Cheat Sheet: Purview Compliance Foundations

### Sensitivity Labels vs DLP Policies
| Feature | Sensitivity Label | DLP Policy |
|---|---|---|
| Purpose | Classify + protect content | Detect + prevent leakage |
| Persists with file? | Yes | No (policy enforced at boundary) |
| Actions | Encrypt, mark, restrict access, container labels | Block, warn/override, notify admin, restrict sharing |
| Applies to | Files, emails, Teams/SharePoint sites (containers) | Exchange, SharePoint, OneDrive, Teams, Endpoint devices, Power BI, 3rd-party apps |

### Data Classification Methods
| Method | Detection Type | Best For |
|---|---|---|
| Sensitive Information Type (SIT) | Pattern (regex, keyword, checksum) | Structured data (SSN, credit card, custom IDs) |
| Trainable Classifier | Machine learning (seed samples) | Unstructured/contextual content (resumes, complaints) |
| Exact Data Match (EDM) | Exact match against a schema of known values | Precise record matching (e.g., customer DB) |

- SIT match confidence: **Low / Medium / High**
- Trainable classifier: start with **~50 seed items** (positive + negative)

### Content Explorer vs Activity Explorer
| Tool | Shows | Time View |
|---|---|---|
| Content Explorer | Current classified content locations | Snapshot (now) |
| Activity Explorer | User actions on labeled content (applied/changed/removed) | Historical timeline |

### Compliance Manager
- Produces a **compliance score** based on completed **improvement actions**
- Action categories: **Preventive / Detective / Corrective**
- Action ownership: **Mandatory / Discretionary**
- Control ownership: **Microsoft-managed / Customer-managed / Shared**
- **Regulatory templates** (GDPR, ISO 27001, NIST, etc.) generate **assessments** with pre-mapped controls

### Sensitivity Label Mechanics
- Label list ordered least → most restrictive; **higher priority (lower in list) wins** when auto-labeling conflicts occur
- **Label policies** control publishing: who sees which labels, default label, mandatory labeling, justification for downgrade
- Auto-labeling can be policy-driven (service side) or user-recommended (client side)

### Common Exam Traps
- Confusing sensitivity labels (protect content) with DLP (prevent leakage action) — they work together, not interchangeably
- Assuming Compliance Score is a single fixed universal number — it's tenant/assessment specific
- Choosing trainable classifier for simple pattern data (should use SIT) or vice versa for free-text context
- Mixing up Content Explorer (current state) with Activity Explorer (historical activity log)

### Portal Note
Microsoft Purview compliance portal = formerly **Microsoft 365 compliance center** (compliance.microsoft.com).
