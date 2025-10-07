# 🗂️ Data Classification & Handling Policy
**APJ Enterprise LLC — NIST SP 800‑171 | DoDI 5200.48 | NIST SP 800‑53 Rev.5 (MP‑2, MP‑4, PL‑2)**

## 1. Purpose
Establish consistent classification, labeling, handling, storage, transmission, and destruction of organizational data.

## 2. Classification Levels
| Level | Description | Examples |
|---|---|---|
| **CUI** | Controlled Unclassified Information requiring safeguarding | Contract data, security configs, audit logs |
| **PII** | Personally Identifiable Information | Names, emails, phone, SSN (if present) |
| **Internal** | Business‑internal information not for public release | Process docs, internal emails |
| **Public** | Approved for public disclosure | Marketing pages, public README |

## 3. Handling Requirements
| Level | Labeling | Storage | Transmission | Destruction |
|---|---|---|---|---|
| CUI | `CUI//NOFORN` or applicable marking | Encrypted at rest | TLS 1.2+; approved recipients only | Shred 1/32" or crypto‑erase |
| PII | `PII` | Encrypted at rest | TLS 1.2+; minimal disclosure | Shred 1/32" or crypto‑erase |
| Internal | `Internal` | Standard controls | TLS recommended | Standard disposal |
| Public | None | N/A | N/A | N/A |

## 4. Roles
- **Data Owner:** Defines level, approves sharing.  
- **Data Custodian:** Implements technical safeguards (encryption, access controls).  
- **Users:** Follow handling rules; report mishandling.

## 5. Exceptions
Document approved exceptions with compensating controls; review quarterly.

---

**Owner:** CISO/ISSM • **Last Updated:** {{UPDATE_DATE}}
