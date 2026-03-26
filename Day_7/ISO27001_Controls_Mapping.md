
# ISO 27001:2022 Controls Mapping  
**Author:** Bozhidar Nikolchev  
**Track:** GRC / Compliance Analyst  
**Day 7 Artifact**

---

## 1. Purpose
Map realistic security risks to ISO 27001:2022 controls and to practical implementations and evidence artifacts used in audits and assessments.

---

## 2. ISO 27001:2022 Control Themes (Overview)
- **A.5 – Organizational controls** (governance, risk, policies, suppliers, classification)
- **A.6 – People controls** (screening, awareness, training, responsibilities)
- **A.7 – Physical controls** (perimeters, entry, secure areas, equipment)
- **A.8 – Technological controls** (auth, encryption, secure coding, logging, config)

> Note: Use your risk assessment to justify which controls apply; Annex A is not a checklist.

---

## 3. Mapping Method
Each mapping includes **Risk → Relevant ISO Controls → Implementation → Evidence**. This mirrors what auditors and internal GRC teams expect.

---

## 4. Mapping: Unauthorized Access to Sensitive Data
**Relevant ISO Controls**  
- A.8.23 Authentication  
- A.8.28 Encryption  
- A.6.3 Information security awareness  
- A.5.17 Identity management  

**Implementation Examples**  
- MFA enforced for all users and privileged roles  
- NIST-aligned password policy  
- Encryption at rest (BitLocker/FileVault) and in transit (TLS 1.2+)  
- Annual training on credential hygiene and phishing  

**Evidence Examples**  
- Azure AD/Google Workspace MFA enforcement report  
- Screenshots of device encryption status  
- Training completion logs and policy acknowledgments

---

## 5. Mapping: Data Leakage via Misconfigured Endpoints
**Relevant ISO Controls**  
- A.8.1 User endpoint protection  
- A.8.9 Configuration management  
- A.8.20 Data masking  
- A.5.20 Supplier relationships security  

**Implementation Examples**  
- CIS baseline applied via MDM (Intune/Jamf/Workspace ONE)  
- Application allow‑listing  
- Regular vulnerability scans and patch SLAs  

**Evidence Examples**  
- MDM compliance reports  
- CIS scan screenshots  
- Agent deployment inventory and patch metrics

---

## 6. Mapping: Ransomware Causing Data Loss
**Relevant ISO Controls**  
- A.5.7 Threat intelligence  
- A.8.15 Logging and monitoring  
- A.8.13 Backup  
- A.6.3 Awareness  
- A.8.2 Anti‑malware protection  

**Implementation Examples**  
- Daily backups with offline/immutable copies  
- SIEM detections for lateral movement and mass encryption behavior  
- Endpoint anti‑malware with tamper protection  
- Phishing/ransomware awareness training  

**Evidence Examples**  
- Backup job success reports and restore test records  
- SIEM alert exports and tuning notes  
- EDR/AV dashboard screenshots

---

## 7. Notes for Reviewers
- Each control is justified by a stated risk and supported by concrete evidence.  
- This format is reusable across systems, vendors, and projects.