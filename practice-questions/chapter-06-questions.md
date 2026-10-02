## Chapter 6: Threat Protection with Microsoft Defender XDR — Practice Questions

**Q1.** A company keeps receiving malicious attachments and phishing links that bypass basic mail filtering. Which Microsoft Defender product should be enabled to add advanced protection against this threat?

A) Microsoft Defender for Cloud Apps
B) Microsoft Defender for Identity
C) Microsoft Defender for Endpoint
D) Microsoft Defender for Office 365

<details>
<summary>Answer</summary>

**Correct: D**

Defender for Office 365 protects email and collaboration workloads with Safe Links (rewrites and time-of-click checks URLs) and Safe Attachments (detonates files in a sandbox).

**Why the others are wrong:**
- Defender for Cloud Apps is a CASB for SaaS app visibility and control, not mail filtering.
- Defender for Identity monitors on-premises Active Directory signals, not email content.
- Defender for Endpoint protects devices via EDR, not inbound email traffic.

</details>

---

**Q2.** A SOC analyst investigates suspicious pass-the-hash activity and lateral movement using an on-premises domain account. Which Defender product surfaced this signal?

A) Microsoft Defender for Cloud Apps
B) Microsoft Defender for Endpoint
C) Microsoft Defender for Office 365
D) Microsoft Defender for Identity

<details>
<summary>Answer</summary>

**Correct: D**

Defender for Identity uses sensors installed on domain controllers and AD FS servers to detect identity-based attacks like pass-the-hash and lateral movement on-premises.

**Why the others are wrong:**
- Defender for Cloud Apps monitors cloud SaaS app usage, not on-prem AD authentication traffic.
- Defender for Endpoint focuses on device-level EDR telemetry, not domain controller traffic analysis.
- Defender for Office 365 is scoped to email and collaboration workloads.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A company wants to discover which unsanctioned SaaS applications employees are using and enforce real-time session controls, such as blocking file downloads from risky apps. Which product BEST meets this need?

A) Microsoft Defender for Cloud
B) Microsoft Defender for Endpoint
C) Microsoft Defender XDR
D) Microsoft Defender for Cloud Apps

<details>
<summary>Answer</summary>

**Correct: D**

Defender for Cloud Apps is Microsoft's CASB solution, offering Cloud Discovery for shadow IT and Conditional Access App Control for real-time session policies.

**Why the others are wrong:**
- Defender for Cloud is a workload protection/CSPM tool for Azure, hybrid, and multi-cloud infrastructure resources, not SaaS app discovery — a common name-confusion trap.
- Defender for Endpoint protects devices, not SaaS application sessions.
- Defender XDR is the umbrella correlation suite, not the CASB engine itself.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Which statement BEST describes Microsoft Defender XDR?

A) A network firewall appliance deployed at the perimeter
B) A dedicated SIEM platform for log storage and hunting queries
C) A unified extended detection and response suite that correlates signals from endpoints, identities, email, and apps into single incidents
D) A compliance tool for regulatory reporting

<details>
<summary>Answer</summary>

**Correct: C**

Defender XDR (formerly Microsoft 365 Defender) is the pre- and post-breach XDR suite that unifies signals from Endpoint, Office 365, Identity, and Cloud Apps into correlated incidents.

**Why the others are wrong:**
- Defender XDR is a cloud security suite, not a network firewall.
- SIEM/hunting at scale with long-term log retention is Microsoft Sentinel, a separate product.
- Compliance reporting is handled by Microsoft Purview, not Defender XDR.

</details>

---

**Q5.** A company needs endpoint detection and response (EDR) and threat and vulnerability management for laptops running Windows, macOS, and Linux. Which product should be deployed?

A) Microsoft Defender for Identity
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Office 365
D) Microsoft Defender for Endpoint

<details>
<summary>Answer</summary>

**Correct: D**

Defender for Endpoint provides EDR, threat and vulnerability management, and attack surface reduction across Windows, macOS, Linux, iOS, and Android devices.

**Why the others are wrong:**
- Defender for Identity is scoped to on-premises AD signals, not device-level protection.
- Defender for Cloud Apps addresses SaaS app visibility, not endpoint devices.
- Defender for Office 365 protects mail and collaboration, not devices.

</details>

---

**Q6.** Where should a security analyst go to view correlated incidents that combine alerts from Defender for Endpoint, Defender for Office 365, and Defender for Identity into a single view?

A) Azure portal
B) Microsoft Entra admin center
C) Microsoft Purview compliance portal
D) Microsoft Defender portal (security.microsoft.com)

<details>
<summary>Answer</summary>

**Correct: D**

The Microsoft Defender portal at security.microsoft.com provides the unified incidents queue that correlates alerts across all Defender XDR workloads.

**Why the others are wrong:**
- The Azure portal manages Azure resources and infrastructure, not the XDR incident queue.
- The Microsoft Entra admin center manages identity configuration, not security incidents.
- The compliance portal focuses on data governance and eDiscovery, not threat incidents.

</details>

---

**Q7.** A company needs Cloud Security Posture Management (CSPM) and workload protection for Azure virtual machines and multi-cloud resources. Which product should they choose?

A) Microsoft Defender for Cloud Apps
B) Microsoft Defender for Cloud
C) Microsoft Defender for Endpoint
D) Microsoft Defender XDR

<details>
<summary>Answer</summary>

**Correct: B**

Microsoft Defender for Cloud is the CSPM and cloud workload protection platform (CWPP) covering Azure, hybrid, and multi-cloud infrastructure resources.

**Why the others are wrong:**
- Defender for Cloud Apps is a CASB for SaaS applications, a frequently confused but different product.
- Defender for Endpoint focuses on individual device EDR, not cloud resource posture.
- Defender XDR correlates identity/endpoint/email/app signals, not infrastructure posture assessment.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** A SOC team wants an AI assistant embedded directly in the Defender portal that can summarize an incident in natural language and suggest remediation steps. Which capability provides this?

A) Microsoft Security Copilot
B) Microsoft Sentinel automation rules
C) Defender for Identity health alerts
D) Microsoft Purview Compliance Manager

<details>
<summary>Answer</summary>

**Correct: A**

Microsoft Security Copilot integrates directly into the Defender portal, using generative AI to summarize incidents, analyze scripts, and recommend remediation in natural language.

**Why the others are wrong:**
- Sentinel automation rules trigger predefined playbooks, not natural-language AI summaries.
- Defender for Identity health alerts report sensor configuration issues, not AI-driven investigation.
- Compliance Manager tracks regulatory compliance scores, unrelated to incident investigation.

</details>

---

