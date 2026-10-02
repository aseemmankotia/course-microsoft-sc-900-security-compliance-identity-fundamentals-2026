# Answer Key — Practice Test 2

**Q1. Correct: D**

Regardless of cloud model (IaaS, PaaS, or SaaS), the customer always retains responsibility for data classification, information/data governance, and access management — this responsibility never shifts to the provider.

---

**Q2. Correct: A**

'Assume breach' means designing systems and segmenting access as if an attacker has already gained a foothold, minimizing blast radius and enabling continuous detection — exactly what is described.

---

**Q3. Correct: B**

Hashing is a one-way function: identical input always yields an identical fixed-length hash value, but the process cannot be reversed to recover the original data — this is why it's used to verify integrity and store passwords securely.

---

**Q4. Correct: A**

Authorization determines what an already-authenticated identity is permitted to do or access; the denial occurs after successful sign-in, meaning the user's permissions — not their identity — caused the failure.

---

**Q5. Correct: B**

Federation establishes a trust relationship between two separate identity providers (Contoso's AD and the partner's IdP) so that authentication tokens issued by one are trusted by the other, without sharing or exposing credentials.

---

**Q6. Correct: D**

Traditional security models assumed everything inside the corporate network firewall was trusted. Zero Trust shifts the perimeter to identity, since users now access resources from anywhere, on any device, over the internet — making network location an unreliable trust signal.

---

**Q7. Correct: C**

PIM provides just-in-time, time-bound privileged role activation that requires justification and can require approval, enforcing zero standing access to admin roles like Global Administrator.

---

**Q8. Correct: A**

Entitlement management lets you bundle multiple resources (groups, apps, SharePoint sites) into an access package that external users can request, with configurable expiration and renewal policies.

---

**Q9. Correct: C**

Identity Protection risk detections can be consumed by Conditional Access sign-in risk policies, which can be scoped to trigger MFA specifically when risk is medium or high, automating the response.

---

**Q10. Correct: D**

Windows Hello for Business provisions a device-bound credential tied to the specific Windows device's TPM, whereas a FIDO2 security key is an external, portable authenticator a user can carry and use to sign in on different compatible devices.

---

**Q11. Correct: A**

Access reviews let you schedule recurring reviews (e.g., every 3 months) of guest user access to resources like Teams/groups, requiring reviewer approval and automatically removing access if not confirmed.

---

**Q12. Correct: C**

Microsoft Entra Verified ID issues decentralized, cryptographically verifiable credentials (such as diplomas) that holders store in a digital wallet and present to relying parties, who can verify authenticity without querying the issuing organization's live systems.

---

**Q13. Correct: C**

PIM provides just-in-time, time-bound activation of privileged roles and supports requiring justification, approval workflows, and MFA before activation — exactly the scenario described.

---

**Q14. Correct: C**

Entitlement management lets administrators bundle multiple resources into an access package that users can self-request through a catalog, with configurable expiration and renewal policies.

---

**Q15. Correct: C**

Access reviews let organizations schedule recurring reviews of group or application access, assign reviewers such as managers, and automatically apply actions like removal if no response is received.

---

**Q16. Correct: A**

Anonymous IP address is a real-time detection in Identity Protection and is classified as Medium risk by default, reflecting a moderate but not maximum confidence indicator of compromise.

---

**Q17. Correct: C**

Microsoft Entra roles control who can manage identity-related resources (users, groups, licenses, directory settings), whereas Azure RBAC controls access to Azure subscription resources like VMs, storage, and networking — they are separate authorization systems.

---

**Q18. Correct: D**

Verified ID issues decentralized, tamper-evident verifiable credentials that holders store in a digital wallet and present to relying parties, who can cryptographically validate authenticity without contacting the original issuer each time.

---

**Q19. Correct: B**

Azure Bastion is a fully managed PaaS service that provides secure RDP/SSH connectivity to VMs directly through the Azure portal over TLS on port 443, without requiring a public IP on the VM, a VPN client, or any open inbound management ports.

---

**Q20. Correct: D**

Azure DDoS Protection Basic is automatically enabled for every Azure resource at no additional cost and provides always-on network-layer traffic monitoring and real-time mitigation of common attacks. DDoS Protection Standard is an additional paid tier enabled per virtual network that adds adaptive tuning based on the network's traffic patterns, near-real-time attack metrics and telemetry via Azure Monitor, and a cost protection SLA guarantee for scale-out costs incurred during a documented attack.

---

**Q21. Correct: B**

Web Application Firewall (WAF) provides centralized, Layer 7 protection for web applications using rule sets (including the OWASP Core Rule Set) specifically designed to detect and block common web exploits such as SQL injection and XSS, and can be deployed with Azure Application Gateway or Azure Front Door.

---

**Q22. Correct: D**

Secure score is a percentage measurement that aggregates the findings of security recommendations across your subscriptions and resources into a single number, weighted by potential impact, so organizations can quickly gauge and prioritize their overall security posture and track improvement over time.

---

**Q23. Correct: B**

Microsoft Sentinel's SOAR (Security Orchestration, Automation, and Response) capability is delivered through automation rules that respond to incidents by triggering playbooks — workflows built on Azure Logic Apps — which can perform actions like isolating a device or disabling a user account automatically without manual analyst intervention.

---

**Q24. Correct: A**

Microsoft Defender for Identity monitors on-premises Active Directory signals — including domain controller traffic and events — to detect identity-based attacks such as pass-the-hash, pass-the-ticket, reconnaissance, and lateral movement, making it the correct choice for this on-premises AD-focused scenario.

---

**Q25. Correct: A**

WAF operates at Layer 7 and includes managed rule sets (based on OWASP Core Rule Set) specifically designed to detect and block SQL injection, XSS, and other web application exploits.

---

**Q26. Correct: A**

Azure Firewall is a managed, cloud-native, stateful network security service that supports FQDN filtering, application/network rules, and threat intelligence-based filtering at a virtual network level.

---

**Q27. Correct: D**

Playbooks, built on Azure Logic Apps, provide the SOAR (Security Orchestration, Automation, and Response) capability in Sentinel, allowing automated actions such as device isolation or account disablement to run when triggered by an alert or incident.

---

**Q28. Correct: C**

Microsoft Sentinel is a cloud-native SIEM/SOAR platform that ingests data from Microsoft and third-party sources across hybrid and multi-cloud environments, correlates it into incidents, and enables threat hunting.

---

**Q29. Correct: A**

Microsoft Defender for Identity monitors on-premises Active Directory signals (via domain controller sensors) to detect identity-based attacks such as pass-the-hash, DCSync, and lateral movement.

---

**Q30. Correct: A**

Microsoft Security Copilot is a generative AI-powered assistant that integrates with Microsoft security products (Defender, Sentinel, Entra, Purview) to help analysts investigate incidents, summarize threat intelligence, and generate response guidance using natural-language prompts.

---

**Q31. Correct: B**

Azure Bastion provides browser-based, TLS-encrypted RDP and SSH access to VMs over port 443 directly through the Azure portal, eliminating the need for public IPs on the VMs.

---

**Q32. Correct: C**

WAF on Application Gateway inspects HTTP/HTTPS requests using OWASP Core Rule Sets, specifically designed to detect and block SQL injection, XSS, and other layer-7 web application attacks.

---

**Q33. Correct: B**

Secure score is calculated from the actual configuration state of resources; the score only increases when the underlying issue is remediated, meaning MFA must genuinely be enabled and enforced.

---

**Q34. Correct: B**

Sentinel's core value is aggregating and correlating logs/signals from across the environment (SIEM), applying analytics for threat detection, and orchestrating automated responses via playbooks (SOAR).

---

**Q35. Correct: D**

Microsoft Security Copilot is a generative AI-powered assistant that integrates with Defender and Sentinel data to summarize incidents, correlate signals across products, and generate natural-language guided remediation steps.

---

**Q36. Correct: C**

Communication Compliance scans internal and external communications for policy violations such as offensive language, harassment, and regulatory conflicts, and routes matches to trained reviewers for investigation and action.

---

**Q37. Correct: C**

Information Barriers define segments of users and policies that explicitly block or allow communication and collaboration between specific groups in Teams, SharePoint, and OneDrive — exactly the conflict-of-interest scenario described.

---

**Q38. Correct: B**

eDiscovery (Premium) extends eDiscovery Standard with end-to-end workflow features including custodian management, review sets, and machine-learning-driven analytics such as near-duplicate detection, email threading, and themes.

---

**Q39. Correct: D**

Event-based retention starts the retention period clock when a defined event occurs (such as contract expiration or an employee's last day), rather than when the label is applied to the content — exactly what's needed here.

---

**Q40. Correct: B**

Discretionary improvement actions are recommended but optional controls — organizations can choose to implement them, and doing so adds points to the overall compliance score, unlike mandatory controls required for certification.

---

**Q41. Correct: D**

Sequence detection in Insider Risk Management identifies patterns of related risky activities occurring over time (such as HR-triggered resignation events followed by data exfiltration behaviors) and correlates them into a single, higher-severity alert.

---

**Q42. Correct: A**

Insider risk management ships with a pre-built 'Data theft by departing users' policy template that ingests HR resignation/termination signals (via HR connector or manual indicators) and correlates them with activity signals like unusual downloads, file uploads to personal cloud storage, and email exfiltration in the weeks before departure — exactly the described use case.

---

**Q43. Correct: B**

eDiscovery (Premium) adds custodian management (including hold notifications and acknowledgment tracking), review sets, and advanced analytics like near-duplicate detection, email threading, and themes — capabilities not present in the lower tiers, making it the only option that satisfies every requirement in the scenario.

---

