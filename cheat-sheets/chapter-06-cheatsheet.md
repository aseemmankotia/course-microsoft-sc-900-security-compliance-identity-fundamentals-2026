## Chapter 6: Microsoft Defender XDR Cheat Sheet

### Defender Product-to-Workload Map (heavily tested)
| Product | Protects | Key Signal/Feature |
|---|---|---|
| Defender for Endpoint | Devices (Windows, macOS, Linux, iOS, Android) | EDR, threat & vuln management, attack surface reduction |
| Defender for Office 365 | Email & collaboration (Exchange, Teams, SharePoint, OneDrive) | Safe Links, Safe Attachments, anti-phishing |
| Defender for Identity | On-premises Active Directory | Sensors on domain controllers/AD FS; detects pass-the-hash, lateral movement |
| Defender for Cloud Apps | SaaS apps (CASB) | Cloud Discovery (shadow IT), Conditional Access App Control (session control) |
| Defender for Cloud (NOT Cloud Apps) | Azure/hybrid/multi-cloud infrastructure | CSPM + CWPP — do not confuse with Cloud Apps |

### Exam Trap: Name Confusion
- **Defender for Cloud** = infrastructure posture (VMs, containers, databases).
- **Defender for Cloud Apps** = SaaS application CASB.
- These are frequently swapped as wrong answers on the exam.

### Microsoft Defender XDR Concept
- Formerly "Microsoft 365 Defender."
- Unifies alerts from Endpoint + Office 365 + Identity + Cloud Apps into **single correlated incidents**.
- Provides pre-breach (posture) and post-breach (detection/response) capability.
- XDR = broader than EDR: correlates across multiple security domains, not just endpoints.

### Microsoft Defender Portal
- URL: **security.microsoft.com**
- Single pane of glass: unified incident queue, hunting, automated investigation & response (AIR).
- Replaces need to check each Defender product console separately.

### Microsoft Security Copilot in Defender Portal
- Embedded generative-AI assistant.
- Capabilities: natural-language incident summarization, script/file analysis, guided remediation recommendations.
- Works across signals surfaced in the Defender portal — not a standalone product deployment per workload.

### Quick Decision Rules
- Keyword **"phishing/email/attachment"** → Defender for Office 365
- Keyword **"device/laptop/EDR"** → Defender for Endpoint
- Keyword **"on-prem AD/domain controller/lateral movement"** → Defender for Identity
- Keyword **"shadow IT/SaaS app/session control"** → Defender for Cloud Apps
- Keyword **"Azure resource/VM posture/multi-cloud"** → Defender for Cloud
- Keyword **"unified incident/single pane"** → Microsoft Defender portal / Defender XDR
- Keyword **"AI summary/natural language investigation"** → Microsoft Security Copilot
