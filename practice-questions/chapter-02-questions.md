## Chapter 2: Microsoft Entra ID: Identities and Authentication — Practice Questions

**Q1.** A company wants employees to be able to reset their own forgotten passwords without contacting the help desk, while still requiring proof of identity through two independent verification methods. Which Microsoft Entra ID feature BEST meets this requirement?

A) Conditional Access policies
B) Privileged Identity Management (PIM)
C) Self-service password reset (SSPR)
D) Identity Protection risk policies

<details>
<summary>Answer</summary>

**Correct: C**

SSPR lets users reset their own password using two configured authentication methods (e.g., mobile app notification + email) without help desk involvement.

**Why the others are wrong:**
- Conditional Access controls access based on signals like location or device, but does not let users reset passwords.
- PIM manages just-in-time privileged role activation, not password resets.
- Identity Protection detects and remediates risky sign-ins/users, it does not provide a self-service reset workflow.

</details>

---

**Q2.** A company needs to grant an external partner organization's employees access to a specific SharePoint site, without creating and managing separate local accounts for them in the tenant. Which solution BEST meets this requirement?

A) Create local user accounts for each partner employee
B) Microsoft Entra External ID for customers (B2C)
C) Microsoft Entra B2B collaboration (guest invitations)
D) Federation with an on-premises AD FS server

<details>
<summary>Answer</summary>

**Correct: C**

B2B collaboration lets external users sign in with their own organizational or social identity as a guest, avoiding the need to create and manage separate credentials.

**Why the others are wrong:**
- Creating local accounts adds administrative overhead and violates the 'no separate accounts' requirement.
- External ID for customers (B2C) is designed for consumer-facing apps, not internal partner collaboration.
- AD FS federation is used to federate an entire on-premises directory with Entra ID, not to grant one-off external partner access to a resource.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** An application running on an Azure Virtual Machine needs to authenticate to Azure Key Vault to retrieve secrets, without any credentials being stored in code or configuration files. Which identity type should be used?

A) Service principal with a client secret
B) Security group
C) Managed identity
D) Guest user account

<details>
<summary>Answer</summary>

**Correct: C**

A managed identity is automatically managed by Entra ID and eliminates the need to store any credentials in code; Azure handles credential rotation behind the scenes.

**Why the others are wrong:**
- A service principal with a client secret requires the secret to be stored and managed somewhere, which violates the 'no stored credentials' requirement.
- Security groups are used to organize identities for access assignment, not to authenticate applications.
- Guest user accounts represent external human users, not application workloads.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** A retail company is building a customer-facing mobile app and wants shoppers to sign up and sign in using their existing Google or Facebook accounts. Which Microsoft Entra offering should the company use?

A) Microsoft Entra External ID (formerly Azure AD B2C)
B) Microsoft Entra B2B collaboration
C) Microsoft Entra Connect
D) Microsoft Entra Privileged Identity Management

<details>
<summary>Answer</summary>

**Correct: A**

External ID for customers (formerly Azure AD B2C) is purpose-built for consumer-facing applications and supports social identity providers like Google and Facebook.

**Why the others are wrong:**
- B2B collaboration is designed for inviting business partners as guests, not for consumer sign-up scenarios.
- Entra Connect synchronizes an on-premises AD with Entra ID; it has nothing to do with customer identity.
- PIM manages privileged role activation for administrators, unrelated to customer sign-in.

</details>

---

**Q5.** A developer registers an application in Microsoft Entra ID and manually manages its credentials (client secret or certificate) so the application can call an API on its own behalf. What identity type does this represent?

A) Service principal
B) Managed identity
C) Dynamic group
D) Device identity

<details>
<summary>Answer</summary>

**Correct: A**

A service principal is the local representation of an app registration in a tenant; when credentials are manually created and managed by the developer, it is a standard service principal, not a managed identity.

**Why the others are wrong:**
- A managed identity's credentials are automatically created and rotated by Azure, not manually managed by a developer.
- Dynamic groups are collections of users/devices based on rules, not application identities.
- Device identities represent registered/joined devices, not applications.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** Which passwordless authentication method relies on public/private key cryptography stored on a dedicated hardware device that a user plugs into or taps against their computer?

A) FIDO2 security key
B) SMS-based one-time passcode
C) Windows Hello for Business
D) OATH hardware token

<details>
<summary>Answer</summary>

**Correct: A**

FIDO2 security keys are external USB/NFC/Bluetooth devices that use public/private key pairs for phishing-resistant passwordless sign-in.

**Why the others are wrong:**
- SMS-based codes are a traditional MFA method, not passwordless, and are not hardware-key based.
- Windows Hello for Business is tied to the specific device via biometrics/PIN, not a separate hardware key.
- OATH hardware tokens generate time-based one-time passcodes for MFA; they are not used for passwordless key-based sign-in.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** An administrator configures Self-Service Password Reset (SSPR) and sets the 'Number of methods required to reset' setting to its default value. How many authentication methods must a user provide to reset their password?

A) 1
B) 2
C) 3
D) 4

<details>
<summary>Answer</summary>

**Correct: B**

The default SSPR configuration requires two authentication methods before a user is allowed to reset their password, increasing security against account takeover.

**Why the others are wrong:**
- Requiring only 1 method is a less secure option that admins can select but is not the default.
- 3 methods is not an available configuration value for this setting.
- 4 methods is not an available configuration value for this setting.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** What is Microsoft Entra ID primarily?

A) A cloud-based identity and access management service
B) An on-premises directory service installed on a Windows Server
C) A network firewall appliance
D) A site-to-site VPN gateway service

<details>
<summary>Answer</summary>

**Correct: A**

Microsoft Entra ID (formerly Azure Active Directory) is Microsoft's cloud-based identity and access management service used to authenticate and authorize users and applications.

**Why the others are wrong:**
- On-premises Active Directory Domain Services, not Entra ID, is installed on Windows Server.
- Entra ID is not a network security appliance.
- Entra ID does not provide VPN connectivity; that is a networking service function.

</details>

---

