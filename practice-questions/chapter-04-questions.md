## Chapter 4: Azure Infrastructure Security and Microsoft Defender for Cloud — Practice Questions

**Q1.** A retail company runs a public-facing e-commerce web app on Azure App Service behind Azure Application Gateway. Recent penetration testing shows the app is vulnerable to SQL injection and cross-site scripting attacks. Which solution BEST addresses this requirement?

A) Configure Network Security Group rules on the App Service subnet
B) Deploy Azure Firewall in front of the Application Gateway
C) Enable Azure DDoS Protection Standard on the virtual network
D) Enable Web Application Firewall (WAF) on the Application Gateway

<details>
<summary>Answer</summary>

**Correct: D**

WAF operates at Layer 7 and includes managed rule sets (OWASP Core Rule Set) specifically designed to block SQL injection, XSS, and other web-layer exploits.

**Why the others are wrong:**
- NSGs filter at Layer 3/4 based on IP/port only — they cannot inspect HTTP payloads for SQL injection patterns
- Azure Firewall is a network/application-layer firewall for outbound/east-west traffic and FQDN filtering, not designed to inspect web request content for OWASP-style exploits
- DDoS Protection defends against volumetric/protocol/resource-layer attacks, not application-layer exploits like SQL injection

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** An administrator needs to allow support staff to RDP into internal VMs for troubleshooting, without assigning public IP addresses to the VMs or opening inbound port 3389 from the internet. Which service BEST meets this requirement?

A) Azure Bastion
B) Azure Firewall with a DNAT rule
C) Network Security Group allowing RDP from the corporate IP range
D) Azure DDoS Protection Standard

<details>
<summary>Answer</summary>

**Correct: A**

Azure Bastion is a fully managed PaaS service that provides RDP/SSH connectivity to VMs directly through the Azure portal over TLS on port 443, with no public IP required on the target VM.

**Why the others are wrong:**
- A Firewall DNAT rule would still expose RDP through a public entry point and requires more management overhead than Bastion
- An NSG rule still requires the VM (or a jump box) to have RDP exposed on a routable path, and doesn't eliminate the need for VM-side public exposure
- DDoS Protection defends against denial-of-service attacks and has no role in providing secure remote access

</details>

---

**Q3.** A financial services company runs a mission-critical trading application on Azure. They require SLA-backed DDoS mitigation, cost protection for scale-out costs incurred during an attack, and access to the DDoS Rapid Response support team. Which DDoS Protection tier should they enable?

A) Azure DDoS Protection Basic
B) Azure DDoS IP Protection only
C) Azure DDoS Protection Standard (Network Protection)
D) Network Security Group with DDoS rules

<details>
<summary>Answer</summary>

**Correct: C**

DDoS Protection Standard (Network Protection) is the paid tier that adds SLA guarantees, cost protection reimbursement for attack-related scale-out, and DDoS Rapid Response support — none of which are included in Basic.

**Why the others are wrong:**
- Basic is automatically enabled and free but provides only platform-level always-on protection with no SLA, cost protection, or rapid response support
- IP Protection is a lighter, per-public-IP paid SKU without the full feature set (e.g., no dedicated Rapid Response access) that Network Protection provides
- NSGs have no DDoS mitigation capability — they are packet filters, not DDoS scrubbing services

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Which network security control operates as a stateful Layer 3/4 packet filter applied directly to a subnet or network interface, and is included at no additional cost in Azure?

A) Azure Firewall
B) Network Security Group (NSG)
C) Web Application Firewall (WAF)
D) Azure Bastion

<details>
<summary>Answer</summary>

**Correct: B**

NSGs are free, stateful Layer 3/4 filters that allow or deny traffic based on source/destination IP, port, and protocol, applied at the subnet or NIC level.

**Why the others are wrong:**
- Azure Firewall is a paid, managed service that operates up to Layer 7 with FQDN filtering and threat intelligence — it is not free
- WAF inspects Layer 7 HTTP traffic for web exploits and is a paid add-on to Application Gateway or Front Door, not a subnet-level packet filter
- Azure Bastion provides secure remote access, not packet filtering

</details>

---

**Q5.** A company has multiple virtual networks across several subscriptions and wants a single managed firewall that provides centralized policy management, FQDN-based outbound filtering, and threat intelligence-based alerting. Which service should they deploy?

A) Network Security Groups on each subnet
B) Azure Firewall with Firewall Manager
C) Web Application Firewall on Application Gateway
D) Azure DDoS Protection Standard

<details>
<summary>Answer</summary>

**Correct: B**

Azure Firewall, managed centrally through Azure Firewall Manager, supports FQDN filtering, threat intelligence feeds, and centralized policy across multiple VNets and subscriptions.

**Why the others are wrong:**
- NSGs must be configured per subnet/NIC individually and have no centralized policy manager or FQDN/threat intelligence capability
- WAF only protects inbound HTTP/HTTPS traffic to web applications — it doesn't provide outbound FQDN filtering or cross-subscription network policy
- DDoS Protection mitigates denial-of-service attacks and has no FQDN filtering or centralized firewall policy features

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** An administrator is deploying Azure Bastion into a virtual network. What is the minimum subnet size required, and what must the subnet be named?

A) /24, named GatewaySubnet
B) /27, named BastionSubnet
C) /26, named AzureBastionSubnet
D) /28, named ManagementSubnet

<details>
<summary>Answer</summary>

**Correct: C**

Azure Bastion must be deployed into a dedicated subnet named exactly AzureBastionSubnet with a minimum size of /26 to accommodate the service's scaling requirements.

**Why the others are wrong:**
- GatewaySubnet is the required name for VPN/ExpressRoute gateways, not Bastion, and /24 is oversized/incorrect naming
- BastionSubnet is an incorrect name — the exact required name is AzureBastionSubnet
- /28 is too small to meet Bastion's minimum sizing requirement and the subnet name is also incorrect

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** In Microsoft Defender for Cloud, the secure score for a subscription is calculated based on which of the following?

A) The number of virtual machines deployed in the subscription
B) The number of Microsoft Defender plans enabled, regardless of recommendations
C) The total monthly spend on Azure Security Center licensing
D) The ratio of completed security recommendations to the total possible points across all applicable recommendations

<details>
<summary>Answer</summary>

**Correct: D**

Secure score is expressed as a percentage representing completed recommendation points out of the maximum achievable points for the resources in scope — remediating recommendations directly raises the score.

**Why the others are wrong:**
- VM count has no direct bearing on the score calculation itself, only the recommendations tied to those VMs do
- Enabling Defender plans exposes more recommendations to act on, but the score only improves when those recommendations are remediated, not merely by enabling the plan
- Secure score is not tied to licensing spend — it is a posture metric, not a cost metric

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** Which term describes the ongoing, automated assessment of an organization's cloud resource configurations against security best practices to identify misconfigurations and reduce attack surface?

A) Cloud Workload Protection (CWP)
B) Security Information and Event Management (SIEM)
C) Identity and Access Management (IAM)
D) Cloud Security Posture Management (CSPM)

<details>
<summary>Answer</summary>

**Correct: D**

CSPM continuously evaluates resource configurations across cloud environments, surfacing misconfigurations and recommendations — this is the foundational capability behind Defender for Cloud's secure score.

**Why the others are wrong:**
- CWP focuses on runtime protection of workloads (VMs, containers, databases) against active threats, not configuration posture assessment
- SIEM (like Microsoft Sentinel) aggregates and analyzes security logs/events for detection and response, not configuration posture scoring
- IAM governs identities, authentication, and access permissions — unrelated to resource configuration posture assessment

</details>

---

