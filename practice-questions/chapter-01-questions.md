## Chapter 1: Foundations: Security, Compliance, and Identity Concepts — Practice Questions

**Q1.** A company moves its customer relationship application from an on-premises data center to a fully managed SaaS offering. Under the shared responsibility model, which security responsibility does the CLOUD PROVIDER take on that the company previously owned on-premises?

A) Classifying and labeling sensitive customer data
B) Managing user accounts and access permissions
C) Setting data retention and compliance policies
D) Patching the application and underlying operating system

<details>
<summary>Answer</summary>

**Correct: D**

In SaaS, the provider owns the entire stack below the application layer, including OS patching, application updates, and physical infrastructure.

**Why the others are wrong:**
- Data classification always remains a customer responsibility across IaaS, PaaS, and SaaS.
- Identity and access management (who gets access to what) is always the customer's job in every model.
- Compliance policy decisions and data governance stay with the data owner (the customer), not the provider.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which statement BEST reflects the Zero Trust guiding principle of 'assume breach'?

A) Grant broad access by default and revoke it only after an incident is confirmed
B) Trust any device or user once they have passed the initial network perimeter firewall
C) Require multifactor authentication only for external users, not internal employees
D) Design systems as if an attacker is already inside the network and minimize blast radius through segmentation and monitoring

<details>
<summary>Answer</summary>

**Correct: D**

'Assume breach' means designing controls (segmentation, encryption, monitoring, least privilege) under the assumption an attacker may already have a foothold, limiting damage and lateral movement.

**Why the others are wrong:**
- Granting broad access by default contradicts least privilege, a separate but related Zero Trust principle.
- Trusting anyone inside the perimeter describes the old castle-and-moat model, the opposite of Zero Trust.
- Zero Trust requires verifying explicitly for ALL users and devices, internal or external, not just external ones.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A user enters a correct username and password, and the system then checks whether that user is a member of the 'Finance-Readers' group before allowing access to a report. Which two security concepts does this scenario demonstrate, in order?

A) Authorization, then authentication
B) Authentication, then authorization
C) Encryption, then hashing
D) Federation, then single sign-on

<details>
<summary>Answer</summary>

**Correct: B**

Verifying username/password proves identity (authentication); checking group membership to decide access to a resource is authorization.

**Why the others are wrong:**
- This reverses the correct order — you must authenticate before authorization can occur.
- Encryption and hashing are data protection concepts, unrelated to this login/access scenario.
- Federation and SSO describe trust relationships between identity providers, not the authenticate-then-authorize flow shown here.

</details>

---

**Q4.** A hospital must ensure patient records stored on disk cannot be read even if the physical storage drives are stolen. Which control should be configured?

A) Hashing of patient records with SHA-256
B) Multifactor authentication for hospital staff
C) Network-layer firewall rules restricting inbound traffic
D) Encryption at rest for the storage volumes

<details>
<summary>Answer</summary>

**Correct: D**

Encryption at rest protects data on physical media so that stolen drives yield unreadable ciphertext without the decryption key.

**Why the others are wrong:**
- Hashing is one-way and used for integrity verification/passwords, not for protecting readable data — hashed records can't be 'decrypted' back for use.
- MFA protects login access, not data on a stolen physical disk that bypasses the login process entirely.
- Firewall rules protect network traffic, not data already extracted from a physical drive.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q5.** Which of the following BEST illustrates the defense in depth model applied to a single web application?

A) Combining a network firewall, host-based antivirus, application input validation, and data encryption together
B) Relying solely on a strong firewall at the network perimeter
C) Using one Global Administrator account shared by the IT team for simplicity
D) Disabling logging to reduce noise and storage costs

<details>
<summary>Answer</summary>

**Correct: A**

Defense in depth layers multiple independent controls (perimeter, host, application, data) so that if one layer fails, others still protect the asset.

**Why the others are wrong:**
- Relying on a single control (the firewall) is the opposite of layered defense — a single point of failure.
- A shared admin account violates least privilege and identity-as-perimeter principles, not defense in depth.
- Disabling logging removes a detective control layer, weakening defense in depth rather than supporting it.

</details>

---

**Q6.** A developer needs to verify that a downloaded software file has not been tampered with in transit. Which technique should be used?

A) Compare the file's hash value against the published hash from the vendor
B) Encrypt the file using AES-256 before comparing
C) Store the file in cold/archive storage tier
D) Enable multifactor authentication on the download portal

<details>
<summary>Answer</summary>

**Correct: A**

Hashing produces a fixed-size fingerprint; comparing hashes verifies integrity — any change to the file produces a different hash.

**Why the others are wrong:**
- Encryption protects confidentiality, not integrity verification, and doesn't confirm tampering.
- Storage tier is unrelated to integrity checking; it only affects cost and access speed.
- MFA protects login access to the portal, not the integrity of a downloaded file.

</details>

---

**Q7.** An employee receives an email appearing to be from the IT helpdesk asking them to click a link and re-enter their password to 'avoid account suspension.' Which threat type does this describe?

A) Ransomware
B) Phishing
C) Distributed denial-of-service (DDoS) attack
D) Brute-force attack

<details>
<summary>Answer</summary>

**Correct: B**

Phishing uses deceptive communications (often email) to trick users into revealing credentials or clicking malicious links.

**Why the others are wrong:**
- Ransomware encrypts a victim's data and demands payment; it does not primarily rely on tricking users into entering credentials via email.
- DDoS floods a service with traffic to make it unavailable; it has no credential-harvesting component.
- Brute-force attacks guess passwords through repeated automated attempts, not social engineering via email.

</details>

---

**Q8.** Which of the following BEST describes the purpose of a Governance, Risk, and Compliance (GRC) framework within an organization?

A) It provides a structured approach to aligning IT actions with business goals, managing risk, and meeting regulatory requirements
B) It replaces the need for technical security controls like firewalls and encryption
C) It is a Microsoft-specific product used only for licensing management
D) It exclusively defines password complexity rules for user accounts

<details>
<summary>Answer</summary>

**Correct: A**

GRC is an organizational discipline covering governance (policies/oversight), risk management (identifying/mitigating risk), and compliance (meeting legal/regulatory obligations).

**Why the others are wrong:**
- GRC works alongside technical controls; it does not replace them — governance sets policy, technical controls enforce it.
- GRC is a general business/security discipline, not a specific Microsoft product or licensing tool.
- Password policy is a narrow technical control, only a tiny subset of what GRC encompasses.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

