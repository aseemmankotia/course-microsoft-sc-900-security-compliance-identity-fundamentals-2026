## Chapter 5 Cheat Sheet: Sentinel SIEM/SOAR

### SIEM vs SOAR
| Term | Full Name | Function |
|---|---|---|
| SIEM | Security Information and Event Management | Collect, aggregate, correlate logs; detect threats |
| SOAR | Security Orchestration, Automated Response | Orchestrate workflows; automate incident response |

**Exam tip:** Microsoft Sentinel = cloud-native SIEM **+** SOAR in one product.

### Sentinel Core Components
| Component | Purpose |
|---|---|
| Data Connector | Ingests logs/events from a source into Sentinel |
| Workbook | Interactive dashboard for visualizing data (built on Azure Monitor Workbooks) |
| Analytics Rule | Detection logic that generates alerts from ingested data |
| Incident | Grouped/correlated alerts representing a potential threat |
| Automation Rule | Determines what playbook runs and when, in response to an incident/alert |
| Playbook | Automated response workflow, built on **Azure Logic Apps** |
| Hunting / Bookmarks | Proactive query-based threat hunting; bookmarks save findings |

### Data Flow (Order Matters for Exam)
1. Data Connector → ingest data
2. Analytics Rule → detect & alert
3. Incident → group related alerts
4. Automation Rule → trigger Playbook
5. Playbook (Logic Apps) → execute automated response

**Common trap:** Exam gives a scenario asking 'what must be configured FIRST' — answer is always the data connector; no downstream feature works without ingested data.

### Microsoft Security Copilot
- Generative AI assistant for security teams.
- Natural-language interface: ask questions, get incident summaries, guided remediation steps.
- Integrates with Sentinel, Defender XDR, Entra, Intune, Purview.
- **Exam tip:** Copilot assists/augments analysts — it does not replace Sentinel's detection or automation engine.

### Sentinel + Defender XDR Integration
- Unified security operations platform: run Sentinel **inside** the Microsoft Defender portal.
- Combines Sentinel's SIEM/SOAR with Defender XDR's cross-workload XDR (endpoint, identity, email, cloud apps) in a single console.
- **Exam trap:** This integration does NOT remove the need for a Log Analytics workspace or data connectors — those remain required underneath.

### Quick Memory Trick
- **S**IEM = **S**ee (visibility/detection)
- **S**OAR = **S**olve (automated action)
- Sentinel = SIEM + SOAR = See + Solve, cloud-native, built on Azure Monitor Log Analytics + Logic Apps.
