# Access Control Policy
Author: Bozhidar Nikolchev  
Version: 1.0  
Status: Draft  
Last Updated: 2026‑03‑22  

---

## 1. Purpose
The purpose of this Access Control Policy is to define how access to organizational systems, data, and resources is governed, controlled, and monitored. This policy ensures that only authorized individuals have appropriate access based on least privilege and need‑to‑know principles.

---

## 2. Scope
This policy applies to:

- All users: employees, contractors, consultants, and third parties  
- All organizational systems, networks, applications, cloud platforms, and databases  
- All data classifications (public, internal, confidential, restricted)  
- All authentication mechanisms, including SSO, MFA, VPN, and IAM solutions  

---

## 3. Access Control Principles

### 3.1 Least Privilege
- Users must be granted only the minimum access required to perform job duties.  
- Elevated or administrative privileges must be strictly controlled and monitored.

### 3.2 Need-to-Know
- Access to sensitive or confidential information is restricted to individuals with a legitimate business need.  

### 3.3 Role-Based Access Control (RBAC)
- Access rights must correspond to predefined organizational roles.  
- Role definitions and permissions must remain documented and periodically reviewed.

---

## 4. Account Management

### 4.1 Account Provisioning
- New accounts must be approved by management and documented.  
- Default passwords must be changed before first use.  
- Access must be aligned to the user’s role.

### 4.2 Account Modification
- Changes in access (promotion, role change, department change) must follow the documented approval process.  
- Changes must be performed within approved timeframes.

### 4.3 Account Deactivation / Termination
- Accounts must be disabled immediately upon termination of employment or contract.  
- Access to sensitive systems must be revoked within SLA (typically same day or within 24 hours).  

---

## 5. Authentication Requirements

### 5.1 Password Requirements
- Passwords must meet complexity standards (length, uniqueness, no reuse).  
- Passwords must not be shared or reused across systems.  
- Password managers are recommended or mandatory depending on systems.

### 5.2 Multi-Factor Authentication (MFA)
MFA is required for:

- Admin and privileged accounts  
- Cloud-based systems  
- VPN and remote access  
- Systems storing confidential or restricted data  

### 5.3 Service and System Accounts
- Non-human accounts must be documented, monitored, and used only for system processes.  
- Passwords or keys for service accounts must be stored securely (e.g., vault).  

---

## 6. Access Reviews

### 6.1 Periodic Reviews
- Access rights must be reviewed at least quarterly or as required by frameworks.  
- Reviewers must confirm access appropriateness and remove any excess privileges.

### 6.2 Privileged Access Reviews
- Admin, root, superuser, and elevated accounts must be reviewed more frequently.  

---

## 7. Monitoring and Logging
- Authentication and access activities must be logged.  
- Logs must be retained according to policy and regulatory requirements.  
- Suspicious access attempts must trigger alerts and be investigated.

---

## 8. Compliance Requirements Mapped
| Framework | Requirement |
|----------|-------------|
| ISO 27001 | A.8 – Access Control |
| NIST CSF | PR.AC – Identity & Access Management |
| PCI‑DSS | Requirement 7 – Access to cardholder data |
| GDPR | Article 25 & 32 – Data protection & security |
| SOC 2 | CC6 – Logical Access Controls |

---

## 9. Enforcement
Violations of this policy may lead to:

- Revocation of access  
- HR disciplinary action  
- Contract termination  
- Legal consequences depending on severity  

---

## 10. Review and Updates
This policy must be reviewed:

- At least annually  
- After major organizational or IT changes  
- After significant security incidents  
- When laws or frameworks update  

---