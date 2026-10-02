## Chapter 7: Microsoft Purview: Compliance Foundations and Data Protection — Practice Questions

**Q1.** A company wants to prevent employees from emailing documents that contain credit card numbers to external recipients, while still allowing the documents to be saved normally on SharePoint. Which capability should be configured?

A) A sensitivity label with encryption
B) A Data Loss Prevention (DLP) policy
C) A trainable classifier
D) A retention label

<details>
<summary>Answer</summary>

**Correct: B**

DLP policies detect sensitive information types (like credit card numbers) and can take rule-based actions such as blocking external email while allowing normal storage.

**Why the others are wrong:**
- A sensitivity label classifies/protects content but doesn't by itself block an email send action based on content match.
- A trainable classifier identifies content categories via ML but doesn't enforce a block/allow action.
- A retention label controls how long content is kept, not how it's shared.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which Microsoft Purview feature provides a percentage-based score along with recommended improvement actions to help an organization manage regulatory and compliance requirements?

A) Compliance Manager
B) Content explorer
C) Insider Risk Management
D) Information barriers

<details>
<summary>Answer</summary>

**Correct: A**

Compliance Manager calculates a compliance score based on completed improvement actions mapped to assessments and regulatory templates.

**Why the others are wrong:**
- Content explorer shows a snapshot of classified content, not a compliance score.
- Insider Risk Management detects risky user behavior, unrelated to scoring compliance posture.
- Information barriers restrict communication between groups, unrelated to scoring.

</details>

---

**Q3.** An organization needs to identify unstructured content such as resignation letters and harassment complaints, which cannot be reliably detected using regular expressions or keyword patterns. Which Microsoft Purview capability should be used?

A) Sensitive information type
B) Trainable classifier
C) Sensitivity label
D) Retention policy

<details>
<summary>Answer</summary>

**Correct: B**

Trainable classifiers use machine learning trained on sample documents to identify content by topic or context, ideal for content that lacks a consistent pattern.

**Why the others are wrong:**
- Sensitive information types rely on pattern matching (regex, keywords, checksums) and are not suited to context-based free-text detection.
- Sensitivity labels classify and protect content but don't perform the detection themselves.
- Retention policies govern lifecycle, not content classification.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** A compliance officer wants to see which users applied, changed, or removed sensitivity labels on documents over the past 30 days. Which tool should they use?

A) Activity explorer
B) Content explorer
C) Compliance Manager assessments
D) Data Loss Prevention alerts

<details>
<summary>Answer</summary>

**Correct: A**

Activity explorer tracks label-related and other data governance activities over time, such as label applied, changed, or removed.

**Why the others are wrong:**
- Content explorer shows a current, in-place snapshot of classified content, not historical user activity.
- Compliance Manager assessments track regulatory improvement actions, not label activity.
- DLP alerts show policy match incidents, not general label lifecycle activity.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** Which action can a Data Loss Prevention (DLP) policy take when it detects a policy match in an outgoing email?

A) Automatically encrypt the mailbox database
B) Apply a retention label to the entire mailbox
C) Block the send and notify the user with an option to override with justification
D) Permanently delete the sensitive information type definition

<details>
<summary>Answer</summary>

**Correct: C**

DLP policy tips can block sensitive content from being sent while allowing users to override with a business justification, or notify admins depending on policy configuration.

**Why the others are wrong:**
- DLP does not encrypt entire mailbox databases; that is a broader Exchange/infrastructure task.
- Retention labels are unrelated to DLP mail-flow actions.
- DLP doesn't delete SIT definitions; it only enforces detection-based actions.

</details>

---

**Q6.** A financial services company must comply with GDPR and wants pre-built control mappings and improvement action recommendations specific to that regulation. Which Compliance Manager feature should they use?

A) A custom sensitivity label policy
B) A trainable classifier trained on GDPR documents
C) An activity explorer filter for GDPR
D) A regulatory template to create a GDPR assessment

<details>
<summary>Answer</summary>

**Correct: D**

Compliance Manager provides regulatory templates (e.g., GDPR, ISO 27001, NIST) that generate assessments with pre-mapped controls and recommended improvement actions.

**Why the others are wrong:**
- Sensitivity label policies control label publishing, not regulatory control mapping.
- Trainable classifiers detect content types, not regulatory compliance controls.
- Activity explorer shows label/content activity, not regulation-specific assessments.

</details>

---

**Q7.** What is the primary purpose of applying a sensitivity label to a document?

A) To automatically delete the document after a set retention period
B) To generate a compliance score improvement action
C) To classify and optionally protect the content (e.g., encryption, watermarking) regardless of where it travels
D) To block the document from being uploaded to any cloud service

<details>
<summary>Answer</summary>

**Correct: C**

Sensitivity labels classify content and can enforce persistent protection such as encryption and content marking that travels with the file.

**Why the others are wrong:**
- Deleting after a retention period is the function of retention labels/policies, not sensitivity labels.
- Sensitivity labels don't directly generate Compliance Manager scores.
- Labels classify/protect content; blocking uploads is a DLP or Conditional Access function.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** A healthcare organization needs to prevent patient record numbers (a custom pattern not included in Microsoft's built-in list) from being shared externally via Teams chat. What should the admin create first before building the DLP policy?

A) A custom trainable classifier only
B) A retention label for patient records
C) An information barrier segment
D) A custom sensitive information type matching the patient record number pattern

<details>
<summary>Answer</summary>

**Correct: D**

Custom sensitive information types let admins define pattern-based detection (e.g., regex) for identifiers not covered by built-in types, which the DLP policy can then reference.

**Why the others are wrong:**
- A trainable classifier is better suited to context-based unstructured content, not a fixed structured pattern like a record number.
- A retention label governs lifecycle, not sharing prevention.
- Information barriers restrict communication between groups, unrelated to detecting a specific data pattern.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

