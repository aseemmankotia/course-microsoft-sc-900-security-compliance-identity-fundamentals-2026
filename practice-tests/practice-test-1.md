# Practice Test 1: SC-900: Security, Compliance & Identity Prep

- **Questions:** 43
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-1.md`. Track results in `score-tracker.md`.

---

**Q1.** A company uses a fully SaaS-based email and collaboration suite hosted by a cloud provider. Under the shared responsibility model, who retains responsibility for classifying data and managing user identities and access, regardless of the service model used?

A) The cloud provider
B) The customer
C) Responsibility is split 50/50 between customer and provider for every service model
D) No one — SaaS providers assume full responsibility for customer data

---

**Q2.** A network engineer configures a firewall to trust all traffic originating from inside the corporate network and only inspects traffic that crosses the network perimeter. This design assumes that being on the internal network is sufficient proof of trustworthiness. Which Zero Trust guiding principle does this design violate?

A) Use least privileged access
B) Assume breach
C) Verify explicitly
D) Use micro-segmentation

---

**Q3.** A user attempts to open a company application and is prompted to enter a username and password before being granted any access to the system. Which security concept does this prompt represent?

A) Authentication
B) Authorization
C) Federation
D) Auditing

---

**Q4.** A company needs a cloud-based service that stores user accounts and group memberships, and that applications can query to authenticate and look up users. Which type of service best meets this requirement?

A) A directory service
B) An identity federation service
C) A certificate authority
D) A hashing algorithm

---

**Q5.** An organization wants to ensure that if a physical disk containing customer records is stolen from a datacenter, the data on it cannot be read by whoever possesses the disk. Which technique should be applied to the stored data to meet this requirement?

A) Encryption at rest
B) Hashing
C) Encryption in transit
D) Data masking

---

**Q6.** Which statement best describes the defense in depth security methodology?

A) All security responsibility is delegated to the cloud provider regardless of deployment model
B) Security is only needed at the network layer
C) Multiple layers of security controls are placed throughout a system, so if one layer is breached, other layers still provide protection
D) A single strong perimeter firewall is sufficient to protect all assets

---

**Q7.** A company wants employees to sign in to their Windows 11 laptops using facial recognition or a PIN that is tied to the specific device, eliminating the need to type a password. Which Microsoft Entra authentication capability BEST meets this requirement?

A) Self-service password reset (SSPR)
B) Microsoft Entra Conditional Access
C) Windows Hello for Business
D) Security defaults

---

**Q8.** An organization wants to grant a user the Global Administrator role only for a scheduled 4-hour maintenance window, requiring manager approval before activation and automatic removal of the role after the window ends. Which Microsoft Entra capability should be used?

A) Privileged Identity Management (PIM)
B) Microsoft Entra ID Protection
C) Access reviews
D) Conditional Access

---

**Q9.** An administrator wants a Conditional Access policy that requires multifactor authentication only when a Global Administrator signs in from outside the corporate network, while allowing normal sign-in from trusted network locations. Which combination of Conditional Access settings achieves this?

A) User assignment: All users; Condition: Device platform; Grant control: Require password change
B) User assignment: Global Administrator role; Condition: Sign-in risk; Grant control: Block access
C) User assignment: Directory role (Global Administrator); Condition: Locations (exclude trusted network); Grant control: Require multifactor authentication
D) User assignment: All guest users; Condition: Client application; Grant control: Require compliant device

---

**Q10.** Which Microsoft Entra ID Governance feature allows organizations to bundle resources such as group memberships, application access, and SharePoint site access into a single item that internal or external users can request through a defined approval workflow?

A) Access reviews
B) Privileged Identity Management
C) Microsoft Entra ID Protection
D) Entitlement management

---

**Q11.** A company frequently onboards external partners who each need temporary access to a specific set of SharePoint sites, a Teams channel, and an application for the duration of a project. The company wants partners to request this bundled access through a self-service catalog, with access automatically expiring when the project ends. Which Microsoft Entra capability should be implemented?

A) Microsoft Entra Conditional Access
B) Self-service password reset
C) Entitlement management
D) Windows Hello for Business

---

**Q12.** A company suspects that several users no longer need access to a Microsoft 365 group that was granted six months ago for a project that has since ended. The company wants a structured process where a designated reviewer periodically evaluates whether each member still needs access, and removes access if not confirmed. Which Microsoft Entra feature should be used?

A) Microsoft Entra ID Protection
B) Access reviews
C) Privileged Identity Management
D) Entitlement management

---

**Q13.** A company wants administrators to have standing accounts in Microsoft Entra ID, but their elevated admin role permissions should only be active for a limited time window when actually needed, with approval required and all activations logged. Which Microsoft Entra capability BEST meets this requirement?

A) Conditional Access policies
B) Microsoft Entra Privileged Identity Management (PIM)
C) Self-service password reset (SSPR)
D) Access reviews

---

**Q14.** An organization needs to give external partners a curated bundle of application access and group memberships through a self-service request-and-approval process, with the access automatically expiring after 90 days unless renewed. Which Microsoft Entra ID Governance feature should be used?

A) Microsoft Entra ID Protection
B) Entitlement management
C) Privileged Identity Management
D) Conditional Access

---

**Q15.** A security team wants Microsoft Entra ID to automatically require multi-factor authentication only when a sign-in attempt is evaluated as medium or high sign-in risk, based on signals like impossible travel or anonymous IP addresses. Which two Microsoft Entra components must be combined to configure this?

A) Self-service password reset with Microsoft Entra roles
B) Microsoft Entra ID Protection risk detection with a Conditional Access risk-based policy
C) Access reviews with entitlement management
D) Windows Hello for Business with Verified ID

---

**Q16.** What is the primary purpose of Microsoft Entra Verified ID?

A) To provide a service for issuing and verifying digital credentials that let individuals and organizations validate claims (such as employment or education) without repeatedly contacting the issuer
B) To enforce phishing-resistant biometric sign-in on Windows devices
C) To automatically reset user passwords using registered security questions
D) To scope granular permissions for administrators managing Microsoft Entra roles

---

**Q17.** A company has hundreds of external guest users in Microsoft Entra ID and wants a recurring process where a resource owner is periodically prompted to confirm whether each guest still needs access to a specific Microsoft 365 group, with automatic removal if not confirmed. Which feature should be configured?

A) Microsoft Entra ID Protection
B) Conditional Access
C) Access reviews
D) Privileged Identity Management

---

**Q18.** An organization wants its Windows 11 corporate laptop users to sign in using a PIN or facial recognition tied to the specific device, avoiding the transmission of a password over the network, while still supporting enterprise-managed key recovery through Microsoft Entra ID. Which authentication method should be recommended?

A) Self-service password reset (SSPR)
B) FIDO2 security keys
C) Microsoft Authenticator app notifications
D) Windows Hello for Business

---

**Q19.** An administrator needs to allow secure RDP and SSH access to Azure virtual machines directly through the Azure portal, without exposing the VMs to public IP addresses or requiring a VPN client. Which Azure service BEST meets this requirement?

A) Azure Firewall
B) Azure DDoS Protection Standard
C) Web Application Firewall
D) Azure Bastion

---

**Q20.** A company hosts a public-facing e-commerce web application on Azure and wants to protect it specifically from SQL injection and cross-site scripting attacks at the HTTP layer. Which Microsoft security capability should they deploy?

A) Azure DDoS Protection
B) Web Application Firewall (WAF)
C) Network Security Groups (NSGs)
D) Azure Bastion

---

**Q21.** In Microsoft Defender for Cloud, what does the 'secure score' represent?

A) The number of security alerts generated in the last 30 days
B) The uptime percentage guaranteed by the Azure SLA for a subscription
C) The count of resources protected by Microsoft Sentinel playbooks
D) A percentage-based measurement of an organization's overall security posture based on completed security recommendations

---

**Q22.** A security operations team wants a single cloud-native solution that can collect security data from across their entire enterprise, use AI to detect threats, and automate incident response with playbooks. Which Microsoft solution should they implement?

A) Microsoft Sentinel
B) Microsoft Defender for Cloud Apps
C) Microsoft Purview
D) Microsoft Entra ID Protection

---

**Q23.** A company's security team wants to detect and investigate on-premises Active Directory attacks such as pass-the-hash and lateral movement, using signals from domain controllers. Which Microsoft Defender XDR component should they use?

A) Microsoft Defender for Endpoint
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Office 365
D) Microsoft Defender for Identity

---

**Q24.** A company currently relies on the free protection automatically applied to all Azure virtual networks. They now want enhanced DDoS mitigation, cost protection guarantees, and access to a rapid response support team during an active attack. What should they enable?

A) Azure Firewall Premium
B) Web Application Firewall with the OWASP rule set
C) Microsoft Defender for Cloud enhanced security features
D) Azure DDoS Protection Standard

---

**Q25.** A company must allow administrators to securely connect via RDP and SSH to Azure virtual machines directly through the Azure portal, without assigning public IP addresses to the VMs or opening inbound ports on the network. Which Azure service BEST meets this requirement?

A) Azure Bastion
B) Azure Firewall
C) Network Security Group (NSG)
D) Azure ExpressRoute

---

**Q26.** A security operations team wants a single cloud-native solution that can collect security data from multiple sources, correlate alerts using analytics, and automatically trigger response playbooks (SOAR) when threats are detected. Which Microsoft service provides this capability?

A) Microsoft Sentinel
B) Microsoft Defender for Cloud
C) Microsoft Purview
D) Microsoft Entra ID Protection

---

**Q27.** A security analyst notices suspicious pass-the-hash activity and unusual lateral movement patterns originating from an on-premises Active Directory environment that is synced to Microsoft Entra ID. Which Microsoft Defender XDR component is designed specifically to detect this type of identity-based attack using signals from on-premises Active Directory?

A) Microsoft Defender for Endpoint
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Identity
D) Microsoft Defender for Office 365

---

**Q28.** A company enables Azure DDoS Protection on its virtual network and wants access to a rapid response support team during an active attack, along with cost protection guarantees for scaled resources during a DDoS event. Which DDoS Protection tier provides these specific features?

A) Azure DDoS Protection Basic
B) Azure Firewall Premium
C) Web Application Firewall
D) Azure DDoS Protection Standard

---

**Q29.** A company runs a public-facing web application and needs to protect it from common layer 7 exploits such as SQL injection and cross-site scripting (XSS), while allowing legitimate HTTP/HTTPS traffic through. Which Azure service is specifically designed for this purpose?

A) Azure DDoS Protection
B) Azure Firewall
C) Web Application Firewall (WAF)
D) Network Security Group (NSG)

---

**Q30.** During an active security incident, a SOC analyst wants to use natural language prompts to quickly summarize an incident, generate a script to remediate an identified threat, and receive AI-generated guidance on next investigation steps within the Microsoft security portal. Which Microsoft capability is designed for this scenario?

A) Microsoft Purview Compliance Manager
B) Microsoft Sentinel Analytics Rules
C) Microsoft Security Copilot
D) Microsoft Entra Permissions Management

---

**Q31.** A company needs administrators to connect to Azure virtual machines using RDP and SSH directly through the Azure portal, without assigning public IP addresses to the VMs or opening inbound ports 3389/22 on the network security group. Which Azure service BEST meets this requirement?

A) Azure Firewall
B) Azure DDoS Protection Standard
C) Azure Web Application Firewall
D) Azure Bastion

---

**Q32.** A security administrator wants a single measurement that reflects the current security configuration of Azure resources and provides prioritized, actionable recommendations to improve it. Which Microsoft Defender for Cloud feature provides this?

A) Azure Policy compliance dashboard
B) Azure Monitor Workbooks
C) Secure score
D) Network Watcher

---

**Q33.** Which statement BEST describes the role of Microsoft Sentinel in an organization's security operations?

A) It is an endpoint detection and response agent installed on individual devices.
B) It is a firewall appliance used to filter inbound and outbound network traffic.
C) It is an identity governance tool used to manage access reviews and entitlements.
D) It is a cloud-native SIEM and SOAR solution that collects security data, detects threats, and enables investigation and automated response across the environment.

---

**Q34.** An organization wants visibility into which cloud SaaS applications employees are using, including unsanctioned 'shadow IT' apps, and wants to apply conditional access-style controls to those cloud apps. Which Microsoft Defender XDR component provides this capability?

A) Microsoft Defender for Endpoint
B) Microsoft Defender for Cloud Apps
C) Microsoft Defender for Office 365
D) Microsoft Defender for Identity

---

**Q35.** Which of the following BEST describes Microsoft Security Copilot?

A) A next-generation firewall appliance for filtering malicious network traffic
B) An identity provider used to authenticate users signing into Microsoft 365
C) A generative AI-powered security assistant that integrates with Microsoft security products to help analysts investigate incidents and respond to threats faster
D) A compliance reporting tool used exclusively for regulatory audit documentation

---

**Q36.** A compliance officer opens the Microsoft Purview compliance portal and sees an overall percentage score along with a list of recommended improvement actions grouped by control. Which Purview capability is being used?

A) Compliance Manager
B) eDiscovery (Premium)
C) Insider Risk Management
D) Communication Compliance

---

**Q37.** A company wants to automatically detect and block emails that contain credit card numbers from being sent to external recipients, while still allowing internal transfers of the same data. Which Purview capability should they configure?

A) Sensitivity labels
B) Data Loss Prevention (DLP) policy
C) Retention policies
D) Communication Compliance

---

**Q38.** An administrator creates a sensitivity label named 'Confidential' and wants any document with this label applied to automatically be encrypted so only members of the Finance group can open it. Which sensitivity label setting enables this?

A) Auto-labeling condition
B) Content marking (headers/footers)
C) Publish to a label policy
D) Encryption with assigned permissions

---

**Q39.** A healthcare organization is subject to regulations requiring that certain patient records be retained for 10 years and be made completely immutable so they cannot be modified or deleted by anyone, including administrators, until the retention period expires. Which Purview capability should they use?

A) Retention label configured as a regulatory record
B) Data Loss Prevention policy
C) Sensitivity label with encryption
D) Communication Compliance policy

---

**Q40.** A security team wants to detect when employees who have submitted resignation letters start downloading unusually large amounts of company data to USB devices, so they can investigate potential data theft before the employee leaves. Which Purview capability is designed for this scenario?

A) Insider Risk Management
B) eDiscovery (Standard)
C) Audit (Standard)
D) Information Barriers

---

**Q41.** An organization's compliance team wants to review Microsoft's independently audited security, privacy, and compliance reports (such as ISO certifications and SOC audit reports) to support their own vendor risk assessments before adopting Microsoft 365. Where should they go to access this information?

A) Microsoft Purview compliance portal
B) Microsoft Service Trust Portal
C) Azure Advisor
D) Microsoft Entra admin center

---

**Q42.** A compliance officer wants to identify employees who may be planning to leave the company and could exfiltrate sensitive data before their departure, without collecting evidence for a legal case. The solution must use pseudonymized user identities during initial analysis to protect employee privacy, and only reveal actual identities once a case requires deeper investigation. Which Microsoft Purview capability BEST meets these requirements?

A) Microsoft Purview eDiscovery (Standard)
B) Microsoft Purview Insider Risk Management
C) Microsoft Purview Audit (Premium)
D) Microsoft Purview Communication Compliance

---

**Q43.** An organization must automatically classify records as they reach the end of a legally required retention period, route them to a compliance team for a disposition review, and generate a certificate of destruction once the records are deleted. Which Microsoft Purview solution provides this capability?

A) Data Loss Prevention (DLP)
B) Records Management
C) Sensitivity labels
D) Microsoft Purview Compliance Manager

---

