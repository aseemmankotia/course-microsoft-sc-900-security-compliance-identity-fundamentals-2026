## Chapter 5: Security Management and SIEM/SOAR with Microsoft Sentinel — Practice Questions

**Q1.** A SOC team wants Microsoft Sentinel to automatically disable a user account and isolate a device the moment a high-severity incident involving credential theft is created, without analyst intervention. Which Sentinel capability should they configure?

A) An automation rule that triggers a playbook
B) A workbook with a threshold alert
C) A hunting query saved as a bookmark
D) A data connector with sync filters

<details>
<summary>Answer</summary>

**Correct: A**

Automation rules trigger playbooks (built on Azure Logic Apps) to take automated actions like disabling accounts or isolating devices — this is the SOAR function of Sentinel.

**Why the others are wrong:**
- Workbooks only visualize data; they cannot take remediation actions.
- Bookmarks save data points during hunting for later reference, they don't automate response.
- Data connectors only ingest data into Sentinel; they have no response capability.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** An organization needs a single cloud-native solution that both collects and correlates security logs from multiple sources AND can automatically orchestrate response actions. Which Microsoft solution BEST meets this requirement?

A) Microsoft Defender for Cloud Apps
B) Microsoft Sentinel
C) Microsoft Purview Compliance Manager
D) Microsoft Entra ID Protection

<details>
<summary>Answer</summary>

**Correct: B**

Microsoft Sentinel is a cloud-native SIEM (collection/correlation) and SOAR (orchestrated automated response) solution in one platform.

**Why the others are wrong:**
- Defender for Cloud Apps is a CASB focused on SaaS app visibility and control, not a full SIEM/SOAR.
- Compliance Manager tracks compliance posture and scores, not security event correlation.
- Entra ID Protection detects identity risk but is not a SIEM/SOAR platform.

</details>

---

**Q3.** A SOC manager wants a customizable, interactive dashboard in Microsoft Sentinel to visualize trends in failed sign-ins over the last 30 days across multiple data sources. Which Sentinel feature should be used?

A) Analytics rules
B) Playbooks
C) Workbooks
D) Incidents

<details>
<summary>Answer</summary>

**Correct: C**

Workbooks provide customizable, interactive dashboards and visualizations of data ingested into Sentinel, built on Azure Monitor Workbooks.

**Why the others are wrong:**
- Analytics rules detect threats and generate alerts/incidents; they don't provide dashboard visualization.
- Playbooks automate response actions, not visualization.
- Incidents are groupings of related alerts for investigation, not dashboards.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** What does the acronym SOAR stand for in the context of Microsoft security solutions?

A) Security Operations and Analytics Reporting
B) Security Orchestration, Automated Response
C) Sentinel Operations Alerting and Remediation
D) System Oversight and Automated Recovery

<details>
<summary>Answer</summary>

**Correct: B**

SOAR = Security Orchestration, Automated Response — it refers to orchestrating workflows and automating incident response.

**Why the others are wrong:**
- This is a plausible-sounding but incorrect expansion of the acronym.
- Sentinel is a product name, not part of the SOAR acronym.
- This distractor swaps 'Orchestration' and 'Response' for unrelated terms.

</details>

---

**Q5.** Microsoft Sentinel playbooks are built on which underlying Azure service?

A) Azure Functions
B) Azure Automation Runbooks
C) Azure Logic Apps
D) Azure Event Grid

<details>
<summary>Answer</summary>

**Correct: C**

Sentinel playbooks are collections of automated actions built on Azure Logic Apps, allowing workflow automation triggered by incidents or alerts.

**Why the others are wrong:**
- Azure Functions can be called within workflows but are not the underlying playbook engine.
- Automation Runbooks are a separate Azure Automation feature, not what Sentinel playbooks use.
- Event Grid handles event routing, not the playbook workflow logic itself.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** During an incident investigation, a Tier 1 analyst wants to type a natural-language question such as 'Summarize this incident and recommend next steps' and receive an AI-generated response referencing Sentinel and Defender data. Which Microsoft solution enables this?

A) Microsoft Purview Data Map
B) Microsoft Entra Verified ID
C) Azure Policy
D) Microsoft Security Copilot

<details>
<summary>Answer</summary>

**Correct: D**

Microsoft Security Copilot is the generative AI assistant that integrates with Sentinel and Defender XDR, letting analysts ask natural-language questions and receive AI-generated incident summaries and guided response recommendations.

**Why the others are wrong:**
- Purview Data Map catalogs data assets for governance, unrelated to AI incident assistance.
- Verified ID issues and verifies digital credentials, not related to SOC investigation.
- Azure Policy enforces resource compliance rules, not AI-assisted security investigation.

</details>

---

**Q7.** Before Microsoft Sentinel can analyze log data from Microsoft Defender for Endpoint, what must first be configured?

A) An analytics rule
B) A hunting bookmark
C) A data connector
D) An automation rule

<details>
<summary>Answer</summary>

**Correct: C**

Data connectors are used to ingest data from sources like Defender for Endpoint into the Sentinel workspace; without a connector, no data is available to analyze.

**Why the others are wrong:**
- Analytics rules run against data already ingested — they cannot function without a connector first.
- Bookmarks save findings during hunting, not used for initial data ingestion.
- Automation rules govern how incidents trigger playbooks, unrelated to data ingestion.

</details>

---

**Q8.** A company has enabled the unified security operations platform, running Microsoft Sentinel within the Microsoft Defender portal. What is the PRIMARY benefit of this integration for the SOC team?

A) It removes the need for a Log Analytics workspace
B) It eliminates the need to configure data connectors
C) It provides a single portal combining Sentinel's SIEM/SOAR capabilities with Defender XDR's extended detection and response
D) It automatically converts all Sentinel playbooks into Defender alerts

<details>
<summary>Answer</summary>

**Correct: C**

The unified security operations platform brings Sentinel's SIEM/SOAR capabilities into the Defender portal, giving analysts one place to see Sentinel incidents alongside Defender XDR's cross-workload detections (endpoint, identity, email, cloud apps).

**Why the others are wrong:**
- Sentinel still relies on a Log Analytics workspace underneath even in the unified portal.
- Data connectors are still required to bring in relevant log sources.
- Playbooks remain Logic Apps-based automation; they are not converted into alerts.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

