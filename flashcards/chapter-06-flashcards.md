## Chapter 6: Threat Protection with Microsoft Defender XDR — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | Which Defender product protects devices (Windows, macOS, Linux, iOS, Android) with EDR? | Microsoft Defender for Endpoint. Exam tip: keyword 'device' or 'endpoint' = this product. |
| 2 | Which Defender product protects email and collaboration tools (Exchange, Teams, SharePoint)? | Microsoft Defender for Office 365. Includes Safe Links and Safe Attachments. Exam tip: keyword 'phishing/attachment' = this product. |
| 3 | Which Defender product monitors on-premises Active Directory for identity-based attacks? | Microsoft Defender for Identity. Uses sensors installed on domain controllers and AD FS servers. Exam tip: keyword 'on-prem AD, lateral movement, pass-the-hash' = this product. |
| 4 | Which Defender product is Microsoft's CASB for SaaS app visibility and shadow IT discovery? | Microsoft Defender for Cloud Apps. Provides Cloud Discovery and Conditional Access App Control. Exam tip: keyword 'shadow IT, SaaS session control' = this product. |
| 5 | Defender for Cloud vs Defender for Cloud Apps — what's the difference? | Defender for Cloud = CSPM/workload protection for Azure/hybrid/multi-cloud infrastructure. Defender for Cloud Apps = CASB for SaaS applications. Exam tip: name similarity is a deliberate trap. |
| 6 | What is Microsoft Defender XDR? | A unified extended detection and response (XDR) suite that correlates signals from Endpoint, Office 365, Identity, and Cloud Apps into single incidents for pre- and post-breach protection. |
| 7 | Where do analysts view unified, correlated incidents across all Defender workloads? | The Microsoft Defender portal at security.microsoft.com. Exam tip: this is the single pane of glass for XDR incidents. |
| 8 | What is Microsoft Security Copilot's role within the Defender portal? | An embedded generative-AI assistant that summarizes incidents in natural language, analyzes scripts/alerts, and recommends remediation steps directly inside the Defender workflow. |
| 9 | Where are Defender for Identity sensors installed? | On domain controllers and AD FS servers to capture authentication traffic for detecting identity attacks. Exam tip: no agent needed on every workstation. |
| 10 | What are Defender for Office 365's two signature protection features? | Safe Links (time-of-click URL rewriting/checking) and Safe Attachments (sandbox detonation of files). Exam tip: know these two names by heart. |
| 11 | What CASB feature does Defender for Cloud Apps use to enforce real-time session controls on SaaS apps? | Conditional Access App Control, a reverse-proxy based session control that can block downloads, uploads, or copy/paste in real time. |
| 12 | What does XDR stand for and what makes it different from EDR? | Extended Detection and Response. Unlike EDR (endpoint-only), XDR correlates signals across multiple domains — endpoints, identities, email, and cloud apps — into unified incidents. |
