# 🛡️ Incident Response Plan (IRP)
**APJ Enterprise LLC — FedRAMP Moderate | NIST SP 800‑53 Rev.5 (IR‑4, IR‑6, IR‑8) | NIST SP 800‑61r2**

## 1. Purpose & Scope
This plan defines how APJ Enterprise LLC detects, responds to, and recovers from cybersecurity incidents affecting systems in scope for **FedRAMP Moderate**.

## 2. Policy Basis
- NIST SP 800‑61r2 (Computer Security Incident Handling Guide)
- NIST SP 800‑53 Rev.5: **IR‑4 (Incident Handling), IR‑6 (Incident Reporting), IR‑8 (Incident Response Plan)**
- FedRAMP Moderate baseline requirements

## 3. Roles & Responsibilities
| Role | Responsibilities |
|---|---|
| ISSM | Approves IRP, declares incident severity, coordinates with AO/leadership |
| ISSO | Maintains IR runbook, documents actions, files reports |
| SysAdmin | Executes containment/eradication steps, collects forensic artifacts |
| Legal/Privacy | Advises on notifications for PII/CUI exposure |
| Communications | Prepares internal/external statements |
| Third‑Party CSPs | Provide logs, evidence, and remediation support per contract/SLA |

## 4. Incident Lifecycle
1. **Detect** → SIEM alerts, user reports, vendor notifications  
2. **Analyze** → Validate indicator, scope affected assets, classify type/severity  
3. **Contain** → Isolate hosts, block IOCs, rotate credentials  
4. **Eradicate** → Remove malware, close vulnerabilities, reimage if needed  
5. **Recover** → Restore services, monitor for re‑occurrence, confirm integrity  
6. **Lessons Learned** → 72‑hour post‑incident review, update playbooks and POA&Ms

## 5. Reporting Timelines
- **Internal:** Notify ISSM/ISSO **immediately** after confirmation.  
- **DoD / Fed partner systems:** Report **within 1 hour** of confirmation to the designated security POC.  
- Document all actions in the Incident Log.

## 6. Classification Matrix (Example)
| Severity | Description | Example Actions |
|---|---|---|
| SEV‑1 (Critical) | Active data exfiltration or widespread outage | Engage full IR team, notify AO, 24/7 ops |
| SEV‑2 (High) | Privileged account compromise, lateral movement | Contain affected accounts, enhanced monitoring |
| SEV‑3 (Moderate) | Isolated malware or misconfiguration | Patch, reimage, user notification |
| SEV‑4 (Low) | Benign alerts, scanning | Tune detection, awareness |

## 7. Evidence & Forensics
- Collect: volatile memory captures, logs (auth, network, EDR), disk images where warranted  
- Chain of custody maintained; preserve hashes for integrity.

## 8. Communications
- All external communications are coordinated via **ISSM + Communications lead**.  
- No public statements without approval.

## 9. Incident Log (Template)
| Time (UTC) | Actor | Action | System(s) | Evidence/Link |
|---|---|---|---|---|
| 2025‑10‑07 15:42 | ISSO | Initial alert triage in SIEM | APP‑WEB‑01 | Sentinel Alert #123 |
| 2025‑10‑07 15:58 | SysAdmin | Isolated host from network | APP‑WEB‑01 | EDR case #456 |

## 10. Incident Report Form (Fill‑in)
**Reporter:**  
**Date/Time (UTC):**  
**Systems Affected:**  
**Indicators Observed:**  
**Containment Actions:**  
**Eradication/Recovery Steps:**  
**Data Impact (CUI/PII):**  
**Notifications Sent (who/when):**  
**Lessons Learned:**  

---

**Review Cadence:** Annual or after SEV‑1/2 incidents.  
**Owner:** ISSM • **Last Updated:** {{UPDATE_DATE}}
