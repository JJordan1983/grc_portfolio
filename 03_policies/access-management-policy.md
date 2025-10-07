# APJ Enterprise LLC  
**Access Management Policy**  
**FedRAMP Moderate | NIST SP 800-53 Rev. 5 | DoD-Aligned**

## 1. Purpose
To ensure logical and physical access to APJ Enterprise LLC systems is controlled, reviewed, and removed according to least-privilege principles.

## 2. Scope
Covers all systems and personnel with access to FedRAMP Moderate-authorized environments.

## 3. Policy

### 3.1 Account Provisioning
- Access is granted only after management approval and completion of security training.  
- Privileged accounts use separate credentials from standard accounts.

### 3.2 Least Privilege
- Users receive only the rights necessary for their job.  
- Temporary elevation requires written approval and is time-bound.

### 3.3 Review and Recertification
- Access rights are reviewed **quarterly** by system owners.  
- Inactive accounts > 30 days are disabled; terminated users’ accounts are removed within 24 hours.

### 3.4 Remote Access
- Remote administrative access requires **MFA** and encrypted channels (SSH v2 or TLS 1.2+).  
- VPN access logs are reviewed weekly.

### 3.5 Monitoring and Audit
- All access events are logged and retained **12 months** minimum.  
- The ISSM reviews anomalies monthly and reports to leadership.

## 4. Roles and Responsibilities
- **ISSM:** Oversees implementation and compliance reporting.  
- **System Owners:** Approve, review, and revoke access.  
- **Users:** Follow approved authorization processes.

## 5. Control Mappings
| Control | Framework | Description |
|----------|------------|-------------|
| AC-1 – AC-6 | NIST SP 800-53 Rev 5 | Access Control Policies & Procedures |
| AC-17 | FedRAMP Moderate | Remote Access |
| AC-19 | FedRAMP Moderate | Mobile Device Access |
| IA-2, IA-4 | NIST SP 800-53 Rev 5 | Identification & Authentication |
| PE-2 | FedRAMP Moderate | Physical Access Authorizations |

## 6. References
- FedRAMP Moderate Baseline (AC & IA Families)  
- DoDI 8520.04 Access Management for DoD IT  
- DoDI 8500.01 Cybersecurity Program  
- NIST SP 800-53 Rev 5 Security Controls
