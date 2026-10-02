# Practice Test 2: SC-900: Security, Compliance & Identity Prep

- **Questions:** 43
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-2.md`. Track results in `score-tracker.md`.

---

**Q1.** A company uses Microsoft 365 (a SaaS offering) exclusively and has no on-premises infrastructure. Under the shared responsibility model, who is responsible for classifying company data and configuring the access permissions that control who can view it?

A) Microsoft, because SaaS shifts all security responsibility to the cloud provider
B) Responsibility is split exactly 50/50 between Microsoft and the customer automatically
C) A third-party compliance auditor appointed by Microsoft
D) The customer, because data classification and access control remain the customer's responsibility in every cloud service model

---

**Q2.** A security team redesigns its network so that a compromised device or credential cannot move laterally to reach other systems, and they continuously monitor for anomalous activity assuming an attacker may already be inside the environment. Which Zero Trust guiding principle does this design primarily reflect?

A) Assume breach
B) Verify explicitly
C) Use least privileged access
D) Defense in depth

---

**Q3.** Which statement accurately describes cryptographic hashing as used in security scenarios such as password storage?

A) Hashing is reversible if you have the correct decryption key
B) The same input always produces the same fixed-length output, but the original input cannot be derived from the hash
C) Hash output length varies depending on the size of the input data
D) Hashing requires a public and private key pair, similar to asymmetric encryption

---

**Q4.** A user successfully signs in to a corporate network using their username, password, and a mobile app approval prompt. Moments later, they attempt to open a file on a restricted network share and receive an 'Access Denied' message. Which security process is responsible for the denial?

A) Authorization
B) Authentication
C) Federation
D) Identity provisioning

---

**Q5.** Contoso wants its employees to sign in with their existing on-premises Active Directory credentials to access a partner organization's cloud application, without the partner ever storing or seeing Contoso employees' passwords. Which concept enables this cross-organizational trust relationship between the two identity providers?

A) Single sign-on (SSO)
B) Federation
C) Directory synchronization
D) Multifactor authentication

---

**Q6.** In a modern Zero Trust architecture, identity is described as the 'primary security perimeter.' This concept represents a shift away from relying primarily on which traditional security boundary?

A) Physical security of data centers
B) Application-layer input validation
C) Data-at-rest encryption
D) The network perimeter, such as firewalls defining a trusted internal network

---

**Q7.** A company wants to eliminate standing administrative access. Global Administrators should have no privileges by default, and must submit a justification and receive approval to activate the role for a maximum of 8 hours only when performing administrative tasks. Which Microsoft Entra capability meets this requirement?

A) Conditional Access with a sign-in frequency policy
B) Microsoft Entra Identity Protection risk policies
C) Microsoft Entra Privileged Identity Management (PIM)
D) Access reviews for Microsoft 365 groups

---

**Q8.** A project team needs external partners to request access to a specific set of resources (a group, a SharePoint site, and an application) through a single request, with access automatically expiring after 90 days unless renewed. Which Microsoft Entra ID Governance feature should be used?

A) Entitlement management access packages
B) Conditional Access terms of use
C) Self-service password reset
D) Microsoft Entra ID Protection

---

**Q9.** An organization wants sign-ins detected as medium or high risk by Microsoft Entra ID Protection to automatically require the user to perform multi-factor authentication before being granted access, without an administrator manually intervening. How should this be configured?

A) Enable Security defaults on the tenant
B) Create a user risk-based Conditional Access policy that blocks access for any risk level
C) Configure a sign-in risk-based Conditional Access policy that requires MFA when risk level is medium or high
D) Set up an access review that runs whenever a risky sign-in is detected

---

**Q10.** Which statement correctly differentiates Windows Hello for Business from a FIDO2 security key in Microsoft Entra ID passwordless authentication?

A) FIDO2 keys require an internet connection to authenticate, while Windows Hello for Business works fully offline
B) Windows Hello for Business is a portable credential usable on any device, while FIDO2 keys are tied to a single registered device
C) FIDO2 security keys can only be used with Azure AD Join, while Windows Hello for Business works only with hybrid join
D) Windows Hello for Business credentials are bound to a specific device, while a FIDO2 security key is portable and can be used to sign in across multiple devices

---

**Q11.** A company grants guest users from a partner organization access to an internal Microsoft Teams site for the duration of a joint project. Compliance requires that every guest's continued access be formally reviewed and re-approved by the project owner every 3 months, with automatic removal if not approved. Which Microsoft Entra feature satisfies this requirement?

A) Microsoft Entra access reviews
B) Conditional Access guest access restrictions
C) Identity Protection user risk policy
D) Privileged Identity Management for groups

---

**Q12.** A university wants to issue digital, tamper-evident diplomas that graduates can store in a digital wallet and present to employers, who can then cryptographically verify authenticity without contacting the university's student records system directly. Which Microsoft Entra capability is designed for this scenario?

A) Microsoft Entra entitlement management
B) Microsoft Entra Permissions Management
C) Microsoft Entra Verified ID
D) Microsoft Entra Identity Governance access reviews

---

**Q13.** A financial services company requires that the Global Administrator role only be active for a specific window of time, requires the requester to provide a business justification, and requires an approver to sign off before the role activates. Which Microsoft Entra capability should be configured to meet these requirements?

A) Conditional Access policy scoped to the Global Administrator role
B) Microsoft Entra Identity Protection risk policy
C) Privileged Identity Management (PIM) role activation settings
D) Access reviews on the Global Administrators group

---

**Q14.** An organization wants external partner users to browse a self-service catalog and request a bundle containing an application, a Microsoft 365 group, and a SharePoint site in one request, with the access automatically expiring after 90 days unless renewed. Which Microsoft Entra feature satisfies this requirement?

A) Microsoft Entra Identity Protection
B) Privileged Identity Management (PIM)
C) Entitlement management access packages
D) Conditional Access policies

---

**Q15.** A company wants managers to be periodically prompted every 90 days to confirm whether guest users still need membership in a Teams-connected Microsoft 365 group, with the option to automatically remove access if the manager does not respond. Which Microsoft Entra feature should be used?

A) Conditional Access
B) Identity Protection risk policies
C) Access reviews
D) Privileged Identity Management (PIM)

---

**Q16.** Microsoft Entra Identity Protection flags a sign-in originating from a known Tor exit node (anonymous IP address). By default, what risk level does Identity Protection assign to this real-time detection?

A) Medium risk
B) No risk — anonymous IPs are not evaluated
C) High risk
D) Low risk

---

**Q17.** Which statement correctly distinguishes Microsoft Entra roles from Azure RBAC (role-based access control) roles?

A) Microsoft Entra roles and Azure RBAC roles are fully interchangeable and manage the same resource types
B) Microsoft Entra roles apply only to guest users, while Azure RBAC applies only to member users
C) Microsoft Entra roles govern administrative access to Entra ID resources such as users, groups, and licenses, while Azure RBAC governs access to Azure resources such as virtual machines and storage accounts
D) Microsoft Entra roles govern Azure resources such as virtual machines, while Azure RBAC governs Entra ID objects such as users and groups

---

**Q18.** A university wants to issue digital diplomas that graduates can store in a digital wallet and present directly to employers, allowing the employer to cryptographically confirm authenticity without contacting the university's registrar office. Which Microsoft Entra capability supports this scenario?

A) Microsoft Entra Identity Protection
B) Microsoft Entra Conditional Access
C) Microsoft Entra Privileged Identity Management
D) Microsoft Entra Verified ID

---

**Q19.** A company runs several Azure virtual machines with no public IP addresses assigned. Administrators need to connect to these VMs via RDP and SSH directly through the Azure portal, over TLS, without deploying a VPN client, opening any inbound ports on the VMs, or exposing them to the public internet at any time. Which service should they deploy?

A) Point-to-Site VPN Gateway
B) Azure Bastion
C) Just-in-time VM access via Microsoft Defender for Cloud
D) Azure Firewall

---

**Q20.** By default, what level of DDoS protection does every Azure virtual network automatically receive, and what must be explicitly enabled to add adaptive tuning, near-real-time attack telemetry/metrics, and cost protection guarantees during an attack?

A) No DDoS protection exists by default; Standard tier must always be purchased for any protection to apply
B) Standard tier is enabled by default at no cost; Basic tier is a legacy paid add-on for enterprises
C) DDoS protection is only available for Azure Front Door endpoints, not virtual networks
D) Basic tier is automatically enabled at no cost with platform-level, always-on traffic monitoring and mitigation; DDoS Protection Standard must be enabled per virtual network to add adaptive tuning, near-real-time telemetry, and cost protection guarantees

---

**Q21.** A public-facing web application hosted behind Azure Application Gateway is being targeted by SQL injection and cross-site scripting (XSS) attempts embedded in HTTP request bodies and query strings. Which Azure security capability is purpose-built to inspect and block these Layer 7 web-based attack patterns?

A) Azure Firewall
B) Web Application Firewall (WAF) deployed with Azure Application Gateway or Azure Front Door
C) Azure Bastion
D) A Network Security Group (NSG) rule blocking inbound port 1433

---

**Q22.** What does the secure score shown in Microsoft Defender for Cloud represent?

A) A single unweighted count of all security alerts generated in the last 30 days
B) An SLA guarantee tied to the regulatory compliance dashboard
C) The total number of resources onboarded to Microsoft Defender for Cloud plans
D) A percentage score that aggregates security recommendations across your resources into a single measure used to track and prioritize security posture improvements

---

**Q23.** A SOC wants Microsoft Sentinel to automatically isolate a compromised device and disable the associated user account the moment a specific high-severity alert fires, without waiting for an analyst to take manual action. Which Sentinel capability enables this automated response?

A) Analytics rules alone, since they can both alert on and remediate incidents
B) Automation rules that trigger playbooks built on Azure Logic Apps to take automated response actions
C) Hunting queries, which run proactively to remediate incidents
D) Workbooks, which visualize data and automatically remediate incidents

---

**Q24.** A security team detects suspicious pass-the-hash activity and lateral movement originating from on-premises Active Directory domain controllers. Which Microsoft Defender XDR component is purpose-built to detect this type of on-premises, identity-based attack using signals collected directly from domain controllers?

A) Microsoft Defender for Identity
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Endpoint
D) Microsoft Defender for Office 365

---

**Q25.** A company hosts a public-facing web application on Azure App Service, fronted by Azure Application Gateway. Recent penetration testing revealed the app is vulnerable to SQL injection and cross-site scripting (XSS) attacks at the HTTP layer. Which Azure security capability should the company enable to BEST mitigate these specific attack types?

A) Web Application Firewall (WAF) on Application Gateway
B) Azure DDoS Protection Standard
C) Network Security Groups (NSGs) on the App Service subnet
D) Azure Firewall with network rules

---

**Q26.** An organization wants a single, centralized network security solution that can filter both inbound and outbound traffic across an entire virtual network using FQDN-based rules, application rules, and Microsoft threat intelligence feeds, while providing a fully stateful firewall as a managed service. Which Azure solution should they deploy?

A) Azure Firewall
B) Network Security Groups (NSGs)
C) Azure Bastion
D) Web Application Firewall (WAF)

---

**Q27.** A security engineer wants Microsoft Sentinel to automatically isolate a compromised device and disable the associated user account whenever a specific high-severity analytics rule fires, without requiring manual analyst intervention each time. Which Sentinel component should be configured to achieve this automated response?

A) Workbooks
B) Hunting queries
C) Analytics rules
D) Playbooks (via Azure Logic Apps)

---

**Q28.** A SOC team needs a cloud-native solution that can collect security signals from Azure, on-premises servers, and non-Microsoft cloud platforms, correlate them into unified incidents, and support proactive threat hunting across the combined data. Which Microsoft solution should they implement?

A) Microsoft Defender for Cloud Apps
B) Microsoft Defender for Endpoint
C) Microsoft Sentinel
D) Microsoft Purview

---

**Q29.** A company suspects an attacker is using compromised on-premises Active Directory credentials to move laterally between domain-joined servers, mimicking legitimate reconnaissance behavior like pass-the-hash and DCSync attacks. Which Microsoft Defender XDR component is specifically designed to detect this type of identity-based, on-premises Active Directory attack behavior?

A) Microsoft Defender for Identity
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Office 365
D) Microsoft Defender for Endpoint

---

**Q30.** Which statement BEST describes the purpose of Microsoft Security Copilot within the Microsoft security ecosystem?

A) It is a generative AI assistant that helps security teams investigate, summarize, and respond to threats faster using natural language, integrated with tools like Defender and Sentinel.
B) It replaces the need for Microsoft Sentinel by independently storing and correlating all security log data.
C) It automatically encrypts all sensitive data classified by Microsoft Purview.
D) It is a licensing add-on that grants unlimited access to all Microsoft Defender XDR workloads.

---

**Q31.** A company runs virtual machines in an Azure virtual network. Administrators need to connect to these VMs using RDP and SSH directly through the Azure portal without exposing public IP addresses on the VMs themselves. Which service should they deploy?

A) Azure Firewall
B) Azure Bastion
C) Web Application Firewall
D) Azure DDoS Protection Standard

---

**Q32.** A company hosts a public-facing web application on Azure and needs protection specifically against SQL injection and cross-site scripting attacks at the HTTP/HTTPS layer. Which capability should they deploy in front of the application?

A) Network Security Group rules
B) Azure DDoS Protection Standard
C) Web Application Firewall (WAF) on Azure Application Gateway
D) Azure Firewall Premium

---

**Q33.** In Microsoft Defender for Cloud, the secure score shows a recommendation 'Enable MFA for subscription owner accounts' worth 10 points. What must occur for the organization's secure score to actually increase by those 10 points?

A) An administrator marks the recommendation as resolved without changing any configuration
B) MFA is enabled and enforced on all subscription owner accounts
C) Defender for Cloud is upgraded to a higher pricing tier
D) The recommendation is exempted from the secure score calculation

---

**Q34.** Which statement BEST describes the primary capability Microsoft Sentinel provides as a cloud-native SIEM and SOAR solution?

A) It replaces Microsoft Defender for Endpoint by scanning device files for malware signatures
B) It collects and correlates security signals across the environment, applies analytics to detect threats, and automates response through playbooks
C) It manages user identity lifecycle and enforces conditional access policies
D) It scans source code repositories for hardcoded secrets before deployment

---

**Q35.** A security analyst wants to quickly investigate a complex multi-stage incident correlated across Microsoft Defender for Endpoint, Microsoft Defender for Identity, and Microsoft Sentinel, using natural language prompts to summarize the attack and get suggested remediation steps rather than manually reviewing each alert. Which Microsoft capability is designed for this scenario?

A) Microsoft Purview Audit
B) Microsoft Entra Permissions Management
C) Azure Policy
D) Microsoft Security Copilot

---

**Q36.** A brokerage firm must monitor Microsoft Teams chats and Exchange email for offensive language, sensitive data sharing, and potential regulatory violations, and route flagged messages to a compliance reviewer for investigation and remediation. Which Microsoft Purview solution BEST meets this requirement?

A) Insider Risk Management
B) Data Loss Prevention
C) Communication Compliance
D) Information Barriers

---

**Q37.** An investment bank's M&A advisory team must be prevented from chatting, calling, or sharing files with the equity trading team in Microsoft Teams to avoid conflicts of interest, while both teams can still freely collaborate with everyone else in the company. Which Microsoft Purview capability enforces this?

A) Conditional Access policies
B) Data Loss Prevention policies
C) Information Barriers
D) Sensitivity labels

---

**Q38.** A company is facing litigation and legal counsel needs to add custodians to a case, place holds on their mailboxes and OneDrive content, then use built-in machine learning to identify near-duplicate documents, email threading, and themes across a large review set before producing evidence. Which capability provides this?

A) eDiscovery (Standard)
B) eDiscovery (Premium)
C) Content Search
D) Audit (Premium)

---

**Q39.** A legal department wants a retention label applied to all signed contracts, but the 7-year retention period should not begin counting down until the contract's expiration date is recorded in the system — not when the label is first applied to the document. Which Microsoft Purview records management feature satisfies this requirement?

A) Adaptive scopes
B) A retention policy
C) A sensitivity label
D) Event-based retention

---

**Q40.** In Microsoft Purview Compliance Manager, an organization implements an improvement action that is classified as 'discretionary' rather than 'mandatory.' What does this classification mean for the organization's compliance score?

A) Discretionary actions cannot be tracked in Compliance Manager at all.
B) Discretionary actions are optional but still contribute points toward the compliance score if implemented.
C) Discretionary actions automatically fail the assessment regardless of implementation.
D) Discretionary actions are required for legal certification and must always be completed.

---

**Q41.** An organization integrates its HR system with Microsoft Purview Insider Risk Management so that when an employee submits a resignation, any large file downloads or unusual data transfers by that user in the following weeks are automatically correlated and escalated into a single elevated-risk alert. Which Insider Risk Management capability is responsible for this correlation?

A) Content explorer
B) Communication compliance analytics
C) Adaptive protection scopes
D) Sequence detection

---

**Q42.** An organization's HR system flags that 12 employees have submitted resignation notices effective in two weeks. The security team wants Microsoft Purview to automatically increase monitoring on these specific users' SharePoint, OneDrive, and email activity to detect potential data exfiltration before their last day, using a built-in policy template designed for exactly this scenario. Which Purview capability should they configure?

A) Insider risk management using the 'Data theft by departing users' policy template
B) Communication compliance with an offensive language policy
C) Data loss prevention with an endpoint DLP policy
D) Information barriers segmenting the departing users' group

---

**Q43.** A company is involved in litigation with 50 custodians. Legal needs to place custodians on hold, send and track hold acknowledgment notifications, review documents in structured review sets, and run analytics such as near-duplicate detection and email threading to reduce review volume. Which Microsoft Purview capability meets ALL of these requirements?

A) Content search
B) eDiscovery (Premium)
C) Audit (Premium)
D) eDiscovery (Standard)

---

