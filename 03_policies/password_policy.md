# APJ Enterprise LLC  
**Password and Authentication Policy**  
**FedRAMP Moderate | NIST SP 800-53 Rev. 5 | DoD-Aligned**

## 1. Purpose
This policy defines password and authenticator requirements for all APJ Enterprise LLC systems operating under the FedRAMP Moderate baseline.

## 2. Scope
Applies to all employees, contractors, and third parties with logical access to APJ Enterprise LLC information systems.

## 3. Policy

### 3.1 Composition and Strength
- Minimum password length: **12 characters**  
- Passphrases are permitted and encouraged.  
- Passwords must not contain the username or personally identifiable information.  
- Systems **shall reject** passwords found in known-compromised lists (NIST SP 800-63B § 5.1.1.2).

### 3.2 Rotation and Reuse
- Rotation is required **only upon compromise** or suspicion of compromise.  
- Password reuse is prohibited for the previous 10 passwords.  

### 3.3 Multi-Factor Authentication (MFA)
- MFA is mandatory for privileged, administrative, and remote accounts.  
- MFA must combine at least two categories: knowledge, possession, or inherence.

### 3.4 Storage and Transmission
- Passwords are hashed using **bcrypt, PBKDF2, scrypt, or Argon2**.  
- Transmission must occur only over **TLS 1.2 or higher**.

### 3.5 Account Lockout
- Accounts lock after **10 failed attempts in 15 minutes** and auto-unlock after 30 minutes or by admin reset.

## 4. Responsibilities
- **System Administrators:** Implement and enforce technical controls.  
- **Users:** Create secure credentials and report suspected compromise.

## 5. Control Mappings
| Control | Framework | Description |
|----------|------------|-------------|
| IA-2, IA-5 | NIST SP 800-53 Rev 5 | Identification & Authentication |
| AC-2 | FedRAMP Moderate | Account Management |
| CM-6 | FedRAMP Moderate | Configuration Settings |
| 800-63B | NIST | Digital Identity Guidelines |

## 6. References
- NIST SP 800-63B: Digital Identity Guidelines  
- FedRAMP Moderate Baseline  
- DoDI 8520.04 Access Management for DoD IT  
- DoDI 8500.01 Cybersecurity
