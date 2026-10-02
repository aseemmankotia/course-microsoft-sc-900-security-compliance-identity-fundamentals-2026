## Chapter 5: Security Management and SIEM/SOAR with Microsoft Sentinel — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | What does SIEM stand for and what does it do? | Security Information and Event Management — collects, aggregates, and correlates log/event data from across an environment to detect threats. Exam tip: SIEM = visibility/detection, SOAR = response. |
| 2 | What does SOAR stand for and what does it do? | Security Orchestration, Automated Response — automates and orchestrates workflows to respond to security incidents. Exam tip: pairs with SIEM; Sentinel provides both in one product. |
| 3 | What is Microsoft Sentinel? | A cloud-native SIEM and SOAR solution that collects data across an enterprise, detects threats, investigates incidents, and automates response. Exam tip: it's the only Microsoft product that is BOTH SIEM and SOAR. |
| 4 | What is a Sentinel Data Connector? | A configuration that ingests log/event data into Sentinel from a source (e.g., Defender for Endpoint, Azure AD, firewalls). Exam tip: no data flows into Sentinel without a connector configured first. |
| 5 | What is a Sentinel Workbook? | An interactive dashboard for visualizing ingested security data, built on Azure Monitor Workbooks. Exam tip: workbooks visualize — they do not detect or automate. |
| 6 | What is a Sentinel Analytics Rule? | A rule that analyzes ingested data against detection logic and generates alerts, which can be grouped into incidents. Exam tip: analytics rules = detection engine of Sentinel. |
| 7 | What is a Sentinel Incident? | A grouping of related alerts that represents a potential security threat requiring investigation. Exam tip: incidents are the unit analysts triage, not individual raw alerts. |
| 8 | What is a Sentinel Playbook? | A collection of automated response actions/workflows, built on Azure Logic Apps, triggered manually or via automation rules. Exam tip: playbooks = the 'SOAR' part of Sentinel. |
| 9 | What underlying Azure service powers Sentinel playbooks? | Azure Logic Apps. Exam tip: exam may ask 'what technology are playbooks built on' — answer is Logic Apps, not Functions or Automation. |
| 10 | What is Microsoft Security Copilot? | A generative AI security assistant that helps analysts investigate incidents, summarize threats, and get natural-language guided response recommendations, integrating with Sentinel and Defender XDR. Exam tip: AI-assisted, natural-language interface for SOC teams. |
| 11 | How does Sentinel integrate with Microsoft Defender XDR? | Sentinel can run within the Microsoft Defender portal as part of the unified security operations platform, combining Sentinel's SIEM/SOAR with Defender XDR's cross-workload extended detection and response in one console. |
| 12 | SIEM vs SOAR — quick distinction | SIEM = collect + correlate + detect (visibility). SOAR = orchestrate + automate response (action). Exam tip: Sentinel is described as delivering BOTH functions in a single cloud-native product. |
