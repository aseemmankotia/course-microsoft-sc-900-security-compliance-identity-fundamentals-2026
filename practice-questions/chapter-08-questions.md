## Chapter 8: Microsoft Purview: Records, Insider Risk, eDiscovery, and Privacy — Practice Questions

**Q1.** A file is subject to a retention policy that deletes content after 3 years and a retention label applied directly to the file that retains it for 7 years. What happens to the file after 3 years?

A) It is deleted because the policy scope always overrides a label
B) It is deleted immediately because two conflicting rules cancel each other out
C) An admin must manually choose which rule applies before any action occurs
D) It is retained until the 7-year label period expires, then deleted

<details>
<summary>Answer</summary>

**Correct: D**

Microsoft Purview conflict resolution principles: retention always wins over deletion, and the longer retention period wins when there's a conflict, so the 7-year label retention applies.

**Why the others are wrong:**
- Policies do not automatically override labels; explicit labels applied to an item are generally favored over container-level policies
- Conflicting rules never simply cancel out and delete content — retention always wins over deletion
- Resolution is automatic based on documented principles; no manual admin decision is required

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A legal team needs to place custodians on hold, build review sets with near-duplicate detection and email threading, and analyze Teams chat data for an active litigation matter. Which tool should they use?

A) Content search
B) eDiscovery (Standard)
C) Communication compliance
D) eDiscovery (Premium)

<details>
<summary>Answer</summary>

**Correct: D**

eDiscovery Premium adds custodian management, review sets, and analytics like near-duplicate detection and email threading, plus deeper Teams data support — capabilities not in Standard or Content search.

**Why the others are wrong:**
- Content search only supports basic keyword search and export with no case management or holds
- eDiscovery Standard supports case management, holds, search, and export, but lacks review sets, analytics, and custodian communications
- Communication compliance detects policy violations in messages; it is not a litigation discovery tool

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A company wants to detect employees sending threatening or harassing messages in Microsoft Teams chats. Which Microsoft Purview solution should be configured?

A) Insider risk management
B) Communication compliance
C) Data loss prevention
D) eDiscovery Premium

<details>
<summary>Answer</summary>

**Correct: B**

Communication compliance uses machine learning classifiers to detect inappropriate content such as harassment, threats, and adult content across Teams, email, and Yammer.

**Why the others are wrong:**
- Insider risk management focuses on data exfiltration and policy violation risks tied to user activity, not message content tone
- DLP protects sensitive information types (like credit card numbers) from being shared, not offensive language
- eDiscovery Premium is for legal investigations and litigation, not ongoing message content monitoring

</details>

---

**Q4.** An organization must retain audited financial records so they cannot be modified, deleted, or reclassified by anyone, including a Global Administrator, until the retention period expires, per a regulatory mandate. Which retention label configuration should be used?

A) Mark the label as a Regulatory Record
B) Mark the label as a Record
C) Apply a retention policy instead of a label
D) Apply a sensitivity label with encryption

<details>
<summary>Answer</summary>

**Correct: A**

Regulatory Record is the most restrictive label type — content cannot be edited, deleted, or have the label removed by anyone, including admins, until the retention period ends.

**Why the others are wrong:**
- A standard Record restricts editing/deleting but can still be reclassified or have the label removed by an authorized admin
- Retention policies apply at the container level and don't provide the item-level immutability required here
- Sensitivity labels control access and encryption, not retention or deletion behavior

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A compliance officer must determine whether an email from 8 months ago was accessed or auto-forwarded, using crucial mailbox audit events. Which auditing solution provides this capability with sufficient log retention?

A) Audit (Standard)
B) Audit (Premium)
C) Content search
D) Compliance Manager

<details>
<summary>Answer</summary>

**Correct: B**

Audit (Premium) provides longer default log retention (365 days, extendable with add-on licensing) and access to high-value crucial events like MailItemsAccessed, which Audit Standard's 180-day retention would not cover for an 8-month-old event.

**Why the others are wrong:**
- Audit Standard retains audit logs for only 180 days by default, insufficient for an 8-month-old event
- Content search finds and exports content but does not provide mailbox activity audit logs
- Compliance Manager tracks compliance posture and controls, not user activity logs

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A vendor risk assessment team needs to review Microsoft's SOC 2 Type II report and ISO 27001 certification for Microsoft 365 services. Where should they find these documents?

A) Microsoft Service Trust Portal
B) Microsoft Purview compliance portal
C) Microsoft Entra admin center
D) Microsoft Defender portal

<details>
<summary>Answer</summary>

**Correct: A**

The Service Trust Portal provides access to independent audit reports, certifications (SOC, ISO), and trust documents describing Microsoft's security and compliance practices.

**Why the others are wrong:**
- The Purview compliance portal is used to configure and monitor an organization's own compliance policies, not download Microsoft's third-party audit reports
- The Entra admin center manages identity and access, not compliance certifications
- The Defender portal manages threat protection, not compliance documentation

</details>

---

**Q7.** Which Microsoft privacy principle states that customers can access, modify, and delete their own data stored in Microsoft cloud services?

A) Transparency
B) Security
C) Control
D) Strong legal protections

<details>
<summary>Answer</summary>

**Correct: C**

Control is the Microsoft privacy principle asserting that customers own and control their data, including the right to access, modify, and delete it.

**Why the others are wrong:**
- Transparency relates to being clear about what data is collected and how it's used, not control over the data itself
- Security relates to protecting data with encryption and controls, not ownership rights
- Strong legal protections refers to respecting local privacy laws, not the customer's direct control

</details>

---

**Q8.** Several employees have submitted resignations. Leadership wants to monitor whether any of them download or exfiltrate large volumes of sensitive data before their last day. Which insider risk management policy template should be used?

A) Data leaks
B) Data theft by departing users
C) Security violations
D) General insider risk template

<details>
<summary>Answer</summary>

**Correct: B**

The Data theft by departing users template is specifically designed to detect exfiltration activity by users who have resignation dates or HR-flagged departure status in the system.

**Why the others are wrong:**
- Data leaks detects general sensitive data sharing outside the organization, not tied specifically to departing employees
- Security violations focuses on security policy tampering, like disabling antivirus, not data exfiltration by leavers
- The general template is a customizable baseline and doesn't specifically target departing-employee risk indicators

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

