# Continuous Monitoring Policy
**APJ Enterprise LLC — FedRAMP Moderate | NIST SP 800‑137 | NIST SP 800‑53 Rev.5 (CA‑7, RA‑5, SI‑2)**

## 1. Purpose
Define cadence and responsibilities for ongoing assessment of security controls, vulnerability scanning, and POA&M maintenance.

## 2. Monitoring Cadence
| Activity | Tool | Frequency | Owner |
|---|---|---|---|
| External vuln scans | Tenable/ACAS | Monthly | Vulnerability Manager |
| Internal agent health | Defender for Endpoint | Daily | SOC |
| Config drift checks | Intune/Group Policy | Weekly | SysAdmin |
| Log aggregation | Sentinel | Continuous | SOC |
| POA&M review | POA&M Tracker | Monthly | ISSO |
| Control assessment spot‑checks | Manual/Automated | Quarterly | ISSM |

## 3. POA&M Lifecycle
1. Identify weakness → 2. Assign owner/date → 3. Mitigate or accept risk → 4. Validate fix → 5. Close & archive evidence.

### POA&M Tracking (Sample)
| Weakness ID | Control | Description | Owner | Planned Completion | Status | Evidence |
|---|---|---|---|---|---|---|
| POAM‑2025‑001 | IA‑5 | Breached‑password screening not enabled | IAM Lead | 2025‑11‑15 | In Progress | Change ticket #321 |
| POAM‑2025‑002 | AC‑17 | MFA missing for VPN break‑glass acct | Network Lead | 2025‑10‑30 | Open | VPN config PR #88 |

## 4. Metrics & Reporting
- Top open POA&Ms by age/severity  
- Patch SLA adherence (Critical ≤ 15 days, High ≤ 30 days)  
- Endpoint coverage (% with EDR)  
- Authentication failures trend & admin activities

## 5. Evidence Retention
- Logs: 12 months minimum (hot + cold storage)  
- Scan results and POA&M exports: 12 months minimum

## 6. Change Management Linkage
Remediation requiring config change follows CM‑3/CM‑4 processes with rollback plan and approvals.

---

**Owner:** ISSO • **Last Updated:** {{UPDATE_DATE}}
