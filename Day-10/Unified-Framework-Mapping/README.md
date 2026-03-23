# Day 10 – Unified Framework Mapping
Author: Bozhidar Nikolchev  
Program: 30-Day Compliance & Security Governance Program

## 📌 Purpose  
This document maps core security and compliance controls across the most common frameworks used by modern companies:  
ISO 27001:2022, NIST CSF 2.0, PCI-DSS v4.0, GDPR, and SOC 2 (AICPA TSC).

This mapping enables:
- Unified control creation  
- Reduced audit duplication  
- Evidence reusability  
- Compliance automation readiness  

---

## ✅ Control Mapping Table

| Control Category     | ISO 27001              | NIST CSF | PCI-DSS | GDPR              | SOC 2 |
|----------------------|------------------------|----------|---------|-------------------|-------|
| Security Policies    | A.5.1                  | ID.GV-1  | 12.1    | Article 32        | CC1.0 |
| Access Control       | A.8                    | PR.AC    | 7       | Article 25        | CC6   |
| Incident Response    | A.5.24 / A.16          | RS.*     | 12.10   | Articles 33–34    | CC7   |
| Asset Management     | A.5.9 / A.7            | ID.AM    | 2       | Article 30        | CC8   |
| Risk Management      | A.5.3 / Clause 6       | ID.RM    | 12.2    | Article 35        | CC3   |

---

## ✅ How to Use This Mapping
1. Select a control category (e.g., Access Control).  
2. Review requirements across frameworks.  
3. Write **one unified internal control**, e.g.:

**Unified Access Control Statement:**  
> “The organization must implement identity and access management processes ensuring least privilege, role‑based access, authentication security, and periodic access review, consistent with regulatory and industry framework requirements.”

4. Attach evidence:  
- Access policy  
- IAM configuration  
- Access review logs  
- MFA enforcement screenshots  

5. Reuse the same evidence for:  
- ISO 27001 audit  
- SOC 2 audit  
- PCI-DSS audit  
- GDPR compliance  
- NIST CSF maturity assessment  

---

## ✅ Next Steps
Next Day (Day 11) you will build:  
✅ Full Security Policies  
✅ Policy folder structure  
✅ Governance package  
✅ Evidence checklist for each policy  

This will become a **portfolio-ready Governance Documentation Pack**.

``