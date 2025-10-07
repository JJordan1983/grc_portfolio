# ⚙️ Model Governance SOP
**APJ Enterprise LLC — NIST AI RMF v1.0 | ISO/IEC 42001 (in progress)**

## 1. Registration & Documentation
- Register each model with: purpose, data sources, training date, hyperparameters, owners, version, and license.  
- Maintain a **Model Card** (description, metrics, limitations).

## 2. Bias & Fairness Testing
- Use representative test sets; evaluate disparate impact where applicable.  
- Record results and mitigations.

## 3. Change Control
- Retraining requires ticket, approval, and rollback plan.  
- Version every model artifact; retain training data hashes.

## 4. Model Review Checklist
| Item | Reviewer | Status | Notes |
|---|---|---|---|
| Model Card completed |  |  |  |
| Dataset consent & rights verified |  |  |  |
| Bias tests executed & passed thresholds |  |  |  |
| Security review (secrets, injection) |  |  |  |
| Monitoring metrics configured |  |  |  |

---

**Owner:** Data Science Lead • **Last Updated:** {{UPDATE_DATE}}
