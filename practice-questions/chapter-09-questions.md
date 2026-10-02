## Chapter 9: Full SC-900 Practice Exam and Time-Management Strategy — Practice Questions

**Q1.** A company wants to ensure that users must satisfy more than one piece of evidence before accessing a sensitive application, but only when they sign in from an unfamiliar location. Which Microsoft Entra capability BEST meets this requirement?

A) Self-service password reset
B) Conditional Access policy with a sign-in risk condition requiring MFA
C) Microsoft Entra Connect
D) Privileged Identity Management role activation

<details>
<summary>Answer</summary>

**Correct: B**

Conditional Access evaluates signals like location/risk and can require MFA only when conditions are met — exactly the 'sometimes MFA' scenario the exam tests repeatedly.

**Why the others are wrong:**
- SSPR only lets users reset their own passwords, unrelated to access control.
- Entra Connect syncs on-prem AD to Entra ID, it doesn't enforce sign-in conditions.
- PIM controls just-in-time privileged role activation, not general app access based on location.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which Zero Trust guiding principle is demonstrated when an organization grants a contractor access only to the three SharePoint files needed for a project, and nothing else?

A) Verify explicitly
B) Assume breach
C) Use least privileged access
D) Defense in depth

<details>
<summary>Answer</summary>

**Correct: C**

Least privileged access limits access to only what is needed — the exact scenario described.

**Why the others are wrong:**
- Verify explicitly refers to authenticating based on all available data points, not scope of access.
- Assume breach refers to segmenting access and minimizing blast radius from an attacker's perspective, not initial grant scope.
- Defense in depth is a layered-security concept, not one of the three Zero Trust principles Microsoft lists.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A security team needs a single dashboard that shows an aggregated security posture score across Azure resources and provides recommendations to harden configurations. Which service should they use?

A) Microsoft Defender for Cloud Secure Score
B) Microsoft Purview Compliance Manager
C) Microsoft Entra ID Protection
D) Microsoft Sentinel

<details>
<summary>Answer</summary>

**Correct: A**

Defender for Cloud's Secure Score aggregates security posture across Azure (and hybrid/multicloud) resources with actionable recommendations.

**Why the others are wrong:**
- Compliance Manager scores regulatory/compliance posture, not resource security configuration.
- Identity Protection scores/flags identity risk, not general Azure resource posture.
- Sentinel is a SIEM/SOAR for threat detection and response, not a posture-scoring dashboard.

</details>

---

**Q4.** An organization must classify and protect documents containing customer credit card numbers so that they are automatically encrypted when detected, regardless of where they are stored. Which Microsoft Purview capability BEST achieves this?

A) eDiscovery
B) Sensitivity labels with auto-labeling policies
C) Communication compliance
D) Insider risk management

<details>
<summary>Answer</summary>

**Correct: B**

Sensitivity labels combined with auto-labeling policies can detect sensitive info types (like credit card numbers) and automatically apply protection/encryption.

**Why the others are wrong:**
- eDiscovery is for identifying and holding content for legal cases, not ongoing protection.
- Communication compliance monitors messages for policy violations, not document encryption.
- Insider risk management flags risky user behavior, it doesn't apply encryption to documents.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** During the SC-900 exam, a candidate encounters a multiple-choice question they are unsure about. What is the BEST time-management strategy recommended for this situation?

A) Spend as long as needed until certain of the correct answer
B) Skip the question entirely and leave it blank
C) Immediately switch answers on every flagged question during review without re-reading them
D) Eliminate obviously wrong options, select the best remaining guess, flag it, and move on

<details>
<summary>Answer</summary>

**Correct: D**

With ~1 minute per question on average, eliminating implausible distractors, making a best guess, flagging, and moving on preserves time for the rest of the exam while leaving the question answered in case time runs out.

**Why the others are wrong:**
- Spending unlimited time on one question risks not finishing the exam.
- Leaving it blank guarantees zero credit; a flagged guess can still be correct.
- Switching every flagged answer without re-reading ignores the reasoning that led to the original choice and can introduce errors.

</details>

---

**Q6.** A company wants employees to be automatically signed out of corporate apps if their device is later reported lost or stolen, without an admin having to reset every password. Which capability addresses this?

A) Password Protection with banned password lists
B) Continuous Access Evaluation combined with Conditional Access
C) Multifactor authentication registration campaign
D) Microsoft Entra ID Governance access reviews

<details>
<summary>Answer</summary>

**Correct: B**

Continuous Access Evaluation revokes sessions near real-time when signals (like device or user risk) change, working with Conditional Access to enforce that revocation.

**Why the others are wrong:**
- Banned password lists prevent weak passwords, unrelated to session revocation.
- MFA registration ensures users can use MFA but doesn't revoke active sessions.
- Access reviews periodically re-certify access on a schedule, not near real-time on device-loss events.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** Which statement correctly distinguishes Microsoft Defender for Office 365 from Microsoft Defender for Endpoint?

A) Defender for Office 365 protects devices; Defender for Endpoint protects email
B) Both products protect only on-premises Exchange servers
C) Defender for Endpoint is a compliance tool, not a security tool
D) Defender for Office 365 protects email and collaboration tools from phishing/malware; Defender for Endpoint protects devices from advanced threats

<details>
<summary>Answer</summary>

**Correct: D**

Defender for Office 365 focuses on email/collaboration threat protection (phishing, malicious links/attachments); Defender for Endpoint focuses on endpoint/device threat detection and response.

**Why the others are wrong:**
- This reverses the actual scope of each product.
- Both products protect cloud and hybrid environments, not exclusively on-prem Exchange.
- Defender for Endpoint is squarely a security (EDR) tool, not a compliance tool.

</details>

---

**Q8.** While reviewing an SC-900 practice exam score report, a candidate notices they scored lowest on the 'Microsoft compliance solutions' domain. What should they do in the final days before the real exam?

A) Focus additional review time on that domain's services (e.g., Purview, Compliance Manager, Service Trust Portal) since it directly impacts overall pass probability
B) Ignore it since it's the smallest weighted domain
C) Retake only questions from the highest-scoring domain to build confidence
D) Assume all domains are weighted equally so no adjustment is needed

<details>
<summary>Answer</summary>

**Correct: A**

Targeting review toward the weakest domain based on practice exam results is the most efficient use of limited prep time and directly raises the weakest score contributing to the pass/fail threshold.

**Why the others are wrong:**
- The compliance domain still carries meaningful weight (roughly 20-25%) and cannot be ignored.
- Reviewing only strong areas wastes time and doesn't address the actual weakness.
- SC-900 domains are NOT equally weighted — always check the current 'Skills measured' breakdown on Microsoft Learn before the exam.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

