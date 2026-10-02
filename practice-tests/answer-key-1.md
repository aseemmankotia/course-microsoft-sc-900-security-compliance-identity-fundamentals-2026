# Answer Key — Practice Test 1

**Q1. Correct: B**

In the shared responsibility model, the customer always retains responsibility for data classification, accountability, endpoints, accounts, and identities — this never shifts to the provider, even in SaaS, where the provider takes on the most responsibility overall.

---

**Q2. Correct: C**

Verify explicitly means every access request should be authenticated and authorized based on all available data points (identity, device, location, etc.), never granted implicit trust just because traffic originates from inside a network boundary.

---

**Q3. Correct: A**

Authentication is the process of proving a user's identity, typically through credentials such as a username and password, before any access decision is made.

---

**Q4. Correct: A**

A directory service (such as Microsoft Entra ID) stores identity information — user accounts, group memberships, and attributes — and is queried by applications to authenticate users and manage access.

---

**Q5. Correct: A**

Encryption at rest protects data stored on physical media (such as disks) by making it unreadable without the correct decryption key, so stolen hardware does not expose the data.

---

**Q6. Correct: C**

Defense in depth uses a layered approach — physical, identity, perimeter, network, compute, application, and data layers — so that if an attacker breaches one layer, additional layers continue to provide protection.

---

**Q7. Correct: C**

Windows Hello for Business provides passwordless sign-in using biometrics (face/fingerprint) or a PIN that is cryptographically tied to the specific device, replacing password entry.

---

**Q8. Correct: A**

Privileged Identity Management provides just-in-time, time-bound activation of privileged roles, including approval workflows and automatic expiration of the elevated access.

---

**Q9. Correct: C**

Targeting the Global Administrator directory role, using a Locations condition that excludes the trusted corporate network, and applying a Require MFA grant control precisely matches the described requirement.

---

**Q10. Correct: D**

Entitlement management uses access packages to bundle multiple resources into a single, requestable item with defined approval workflows and expiration settings.

---

**Q11. Correct: C**

Entitlement management access packages let organizations bundle resources into a self-service catalog that external users can request, with configurable expiration policies suited to project-based partner access.

---

**Q12. Correct: B**

Access reviews allow a designated reviewer to periodically recertify group membership and automatically remove access from members whose continued need is not confirmed.

---

**Q13. Correct: B**

PIM provides just-in-time, time-bound activation of privileged roles with approval workflows, justification, and full audit history, exactly matching the requirement.

---

**Q14. Correct: B**

Entitlement management lets administrators define access packages bundling resources, with request/approval workflows and expiration policies, ideal for onboarding external users with time-limited access.

---

**Q15. Correct: B**

Identity Protection calculates real-time sign-in risk levels, and a Conditional Access policy can be configured with a sign-in risk condition to require MFA when risk is medium or high — this is the standard risk-based Conditional Access pattern tested on the exam.

---

**Q16. Correct: A**

Verified ID is Microsoft's decentralized identity solution that enables organizations to issue verifiable credentials and lets relying parties verify claims about a person without contacting the original issuer each time, at a conceptual level for SC-900.

---

**Q17. Correct: C**

Access reviews allow organizations to schedule recurring reviews of group, application, or role assignments, letting designated reviewers approve or deny continued access, with automatic removal of access when not confirmed.

---

**Q18. Correct: D**

Windows Hello for Business provides device-bound, passwordless sign-in using a PIN or biometrics, backed by asymmetric key pairs, and integrates with Microsoft Entra ID for enterprise-managed provisioning and recovery.

---

**Q19. Correct: D**

Azure Bastion is a fully managed PaaS service that provides secure RDP and SSH connectivity to VMs directly through the Azure portal over TLS, eliminating the need for public IPs on the VMs or a client-side VPN.

---

**Q20. Correct: B**

Web Application Firewall, available with Azure Application Gateway or Azure Front Door, inspects HTTP/HTTPS traffic and uses managed rule sets (based on OWASP core rules) to block common web exploits such as SQL injection and cross-site scripting.

---

**Q21. Correct: D**

Secure score in Microsoft Defender for Cloud aggregates security recommendations across your environment into a single percentage score, giving an at-a-glance measure of your current security posture and showing the impact of remediating specific recommendations.

---

**Q22. Correct: A**

Microsoft Sentinel is a cloud-native SIEM and SOAR solution that aggregates security data from across an organization, applies AI and analytics for threat detection and investigation, and supports automated response through playbooks built on Azure Logic Apps.

---

**Q23. Correct: D**

Microsoft Defender for Identity monitors on-premises Active Directory signals (via domain controller sensors) to detect identity-based attacks such as pass-the-hash, lateral movement, and reconnaissance activity.

---

**Q24. Correct: D**

Azure DDoS Protection Standard builds on the free, always-on Basic tier by adding tuned mitigation policies specific to the customer's resources, cost protection for scaled-out resources during an attack, and access to the DDoS Rapid Response support team.

---

**Q25. Correct: A**

Azure Bastion is a fully managed PaaS service that provides secure RDP/SSH connectivity to VMs directly through the Azure portal over TLS, eliminating the need for public IPs or open inbound ports on the VMs.

---

**Q26. Correct: A**

Microsoft Sentinel is Microsoft's cloud-native SIEM and SOAR solution. It collects data across the environment, uses analytics and AI to detect threats, and can automate responses through playbooks built on Azure Logic Apps.

---

**Q27. Correct: C**

Microsoft Defender for Identity monitors on-premises Active Directory signals (via sensors on domain controllers) to detect advanced threats such as pass-the-hash, lateral movement, and domain dominance attempts.

---

**Q28. Correct: D**

Azure DDoS Protection Standard adds capabilities beyond the free Basic tier, including access to the DDoS Rapid Response (DRR) support team during an active attack and cost protection for resources that autoscale due to a documented DDoS attack.

---

**Q29. Correct: C**

Web Application Firewall (WAF), deployed with Azure Application Gateway or Azure Front Door, inspects HTTP/HTTPS traffic at layer 7 and blocks common web exploits like SQL injection and XSS using managed rule sets (e.g., OWASP Core Rule Set).

---

**Q30. Correct: C**

Microsoft Security Copilot is a generative AI-powered security assistant that integrates with Microsoft security products, allowing analysts to use natural language prompts to summarize incidents, generate remediation scripts, and receive step-by-step investigation guidance.

---

**Q31. Correct: D**

Azure Bastion provides secure, seamless RDP/SSH connectivity to VMs directly through the Azure portal over TLS, without requiring a public IP on the VM or opening RDP/SSH ports to the internet.

---

**Q32. Correct: C**

Secure score in Microsoft Defender for Cloud aggregates security recommendations into a single score, showing overall posture and prioritizing which actions will most improve security.

---

**Q33. Correct: D**

Microsoft Sentinel is a cloud-native Security Information and Event Management (SIEM) and Security Orchestration, Automated Response (SOAR) solution that aggregates signals from across an environment for detection, investigation, and response, including automated playbooks.

---

**Q34. Correct: B**

Microsoft Defender for Cloud Apps is a Cloud Access Security Broker (CASB) that discovers shadow IT SaaS usage, assesses app risk, and enforces session and access controls over cloud applications.

---

**Q35. Correct: C**

Microsoft Security Copilot is a generative AI assistant that integrates with Microsoft security tools such as Defender XDR and Sentinel, helping security teams summarize incidents, investigate threats, and generate response guidance using natural language prompts.

---

**Q36. Correct: A**

Compliance Manager calculates a compliance score based on completed improvement actions across Microsoft-managed, technical, and organizational controls, giving a percentage score and prioritized recommendations.

---

**Q37. Correct: B**

DLP policies detect sensitive information types like credit card numbers and can enforce different actions (block, warn, allow) based on context such as the recipient being internal or external.

---

**Q38. Correct: D**

Sensitivity labels support encryption settings where you can assign specific users or groups permissions (e.g., view, edit) so only those users can open protected content, regardless of where the file is sent.

---

**Q39. Correct: A**

Records management lets you configure a retention label as a 'regulatory record,' which locks the content so it cannot be edited or deleted by anyone, including admins, until the retention period ends—ideal for strict regulatory retention needs.

---

**Q40. Correct: A**

Insider Risk Management uses signals like resignation and unusual data movement (e.g., mass downloads to USB) to identify potential insider risks, correlating HR and activity data to flag risky behavior for investigation.

---

**Q41. Correct: B**

The Microsoft Service Trust Portal provides access to audit reports, compliance guides, and independent certifications (ISO, SOC, etc.) so customers can assess Microsoft's compliance posture for their own regulatory needs.

---

**Q42. Correct: B**

Insider Risk Management is purpose-built to detect and act on risky behaviors like data theft by departing employees, and it uses pseudonymization by default so investigators see anonymized usernames until a case is escalated and identities need to be revealed.

---

**Q43. Correct: B**

Records Management in Microsoft Purview lets organizations apply retention labels tied to file plans, trigger disposition review workflows when retention periods expire, and produce a certificate of destruction/disposition documenting when content was deleted.

---

