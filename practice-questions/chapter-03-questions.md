## Chapter 3: Microsoft Entra: Access Management and Identity Governance — Practice Questions

**Q1.** A company's security team wants Global Administrator access to be granted only when an admin actively needs it, for a maximum of 8 hours, with a required justification and manager approval. Which Microsoft Entra feature should they configure?

A) Conditional Access with a sign-in frequency control
B) Microsoft Entra ID Protection risk policies
C) Privileged Identity Management (PIM) with eligible assignments
D) Entitlement management access packages

<details>
<summary>Answer</summary>

**Correct: C**

PIM lets you assign roles as 'eligible' rather than permanently active. The user must activate the role, provide justification, and can be required to get manager approval, with the activation automatically expiring after a set duration.

**Why the others are wrong:**
- Conditional Access controls how a session is granted (e.g., require MFA), not time-bound role activation.
- Identity Protection evaluates risk on sign-ins and users, it doesn't manage role activation duration.
- Entitlement management grants access to resource bundles (apps/groups/sites), not built-in admin roles with time-bound elevation.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A user's credentials were found for sale on a known dark web marketplace. Microsoft Entra ID Protection flags this. What type of risk detection is this?

A) User risk
B) Sign-in risk
C) Session risk
D) Application risk

<details>
<summary>Answer</summary>

**Correct: A**

User risk reflects the probability that the identity itself (the account) has been compromised, based on signals like leaked credentials, regardless of any specific sign-in attempt.

**Why the others are wrong:**
- Sign-in risk evaluates the probability that a specific authentication request isn't authorized by the legitimate owner (e.g., anonymous IP, impossible travel), not stolen credential exposure.
- 'Session risk' is not a Microsoft Entra ID Protection risk category.
- 'Application risk' is not a defined Microsoft Entra ID Protection risk category.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** An organization onboards external partners frequently and wants them to self-service request access to a curated bundle of three apps and a SharePoint site, with automatic expiration and manager approval, without IT manually adding each partner to each resource.

A) Create a Conditional Access policy targeting guest users
B) Configure Microsoft Entra ID Protection for external identities
C) Create an access package using entitlement management
D) Assign the partners as eligible members via Privileged Identity Management

<details>
<summary>Answer</summary>

**Correct: C**

Entitlement management access packages bundle multiple resources (apps, groups, SharePoint sites) into a single self-service request with approval workflows and automatic access expiration — purpose-built for this scenario.

**Why the others are wrong:**
- Conditional Access controls authentication conditions, it cannot bundle or provision resource access.
- Identity Protection detects and responds to risk; it doesn't grant or bundle resource access.
- PIM manages just-in-time privileged role activation, not standard resource access for external partners.

</details>

---

**Q4.** Which Microsoft Entra ID capability requires a Microsoft Entra ID P1 license and lets an admin block or grant access based on signals such as device compliance, location, and application?

A) Identity Protection
B) Conditional Access
C) Privileged Identity Management
D) Access reviews

<details>
<summary>Answer</summary>

**Correct: B**

Conditional Access is the P1-licensed feature that evaluates signals (user, location, device, application, risk) to make an access decision (allow, block, or require controls like MFA).

**Why the others are wrong:**
- Identity Protection uses risk signals but requires Microsoft Entra ID P2, not P1.
- PIM requires Microsoft Entra ID P2 and manages role activation, not general sign-in access decisions.
- Access reviews are part of Entra ID Governance/P2, used for periodic recertification, not real-time access decisions.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** A compliance team needs group owners to periodically recertify whether external guest users still need access to a Microsoft 365 group, and automatically remove access if not confirmed. Which feature satisfies this requirement?

A) Conditional Access terms of use
B) Entitlement management access packages
C) Access reviews
D) Microsoft Entra ID Protection risk policies

<details>
<summary>Answer</summary>

**Correct: C**

Access reviews (part of Microsoft Entra ID Governance) let designated reviewers periodically confirm or reject continued access to groups, apps, or roles, with automatic removal on denial or non-response.

**Why the others are wrong:**
- Terms of use requires users to accept a policy statement; it does not recertify ongoing access.
- Access packages grant initial access via request/approval; they aren't the recurring recertification mechanism itself (though reviews can be attached to them).
- Risk policies respond to detected sign-in/user risk, not scheduled access recertification.

</details>

---

**Q6.** In a Conditional Access policy, which component determines the outcome applied to a sign-in attempt, such as requiring multi-factor authentication or blocking access?

A) Grant controls (decisions)
B) Signals
C) Session controls only
D) Named locations

<details>
<summary>Answer</summary>

**Correct: A**

Grant controls are the decision component of a Conditional Access policy — they define what must happen (block, require MFA, require compliant device, etc.) once the assignment conditions match.

**Why the others are wrong:**
- Signals (user, location, device, application, risk) are inputs evaluated to decide whether the policy applies, not the resulting action.
- Session controls limit what a user can do within a session (e.g., limited browser access); they are one enforcement option, not the entire decision component.
- Named locations are a single type of signal used in conditions, not the decision itself.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** In Microsoft Entra Privileged Identity Management, what does an 'eligible' role assignment mean for the assigned user?

A) The user has the role permissions active at all times
B) The user must perform an activation step before the role's permissions become active, and access expires after a set time
C) The user's access request is pending administrator approval and has no permissions yet
D) The user was denied the role due to a detected risk

<details>
<summary>Answer</summary>

**Correct: B**

An eligible assignment in PIM means the role is not active by default; the user must activate it (optionally with MFA, justification, or approval), and the elevated permissions automatically expire after a configured duration.

**Why the others are wrong:**
- That describes an 'active' assignment, not 'eligible'.
- Eligible does not mean pending approval by default — activation may or may not require approval depending on policy, but the assignment already exists.
- Eligible assignment is unrelated to risk denial; it's a standard PIM assignment type.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** What is Microsoft Entra Verified ID primarily used for?

A) Enforcing multi-factor authentication for privileged roles
B) Scanning for leaked credentials on the dark web
C) Issuing and verifying decentralized, portable digital credentials based on open standards
D) Managing time-bound activation of Azure resource roles

<details>
<summary>Answer</summary>

**Correct: C**

Microsoft Entra Verified ID enables organizations to issue and verify digital credentials (such as proof of employment or education) using decentralized identity and open W3C Verifiable Credentials standards, giving individuals control over their own credentials.

**Why the others are wrong:**
- MFA enforcement is handled by Conditional Access/authentication methods, not Verified ID.
- Dark web credential scanning is part of Identity Protection's user risk detection, not Verified ID.
- Time-bound role activation describes PIM, not Verified ID.

</details>

---

