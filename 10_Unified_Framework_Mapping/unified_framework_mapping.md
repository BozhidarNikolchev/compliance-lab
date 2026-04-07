# Day 10 – Unified Framework Mapping
Author: Bozhidar Nikolchev  
Program: 30-Day Compliance & Security Governance Program

## 📌 Purpose  
This document maps core security and compliance controls across major frameworks:  
- ISO 27001:2022  
- NIST CSF 2.0  
- PCI-DSS v4.0  
- GDPR  
- SOC 2 (AICPA Trust Services Criteria)

The goal is to:
- Reduce audit duplication  
- Reuse evidence across audits  
- Create unified internal controls  
- Support compliance automation  

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

## ✅ Unified Control Creation (How to Use)

1. Select a category (e.g. Access Control)  
2. Compare requirements across frameworks  
3. Create **one unified internal control**, e.g.:

**Unified Access Control Statement:**  
> “The organization must implement identity and access management processes ensuring least privilege, role-based access, authentication security, and periodic access reviews, consistent with regulatory and industry framework requirements.”

4. Attach evidence such as:  
- IAM policy  
- Access review logs  
- MFA screenshots  
- User provisioning workflows  

5. Reuse the same evidence across:  
- ISO 27001 audit  
- SOC 2 assessment  
- PCI-DSS controls  
- GDPR accountability (Art. 5, 25, 32)  
- NIST CSF maturity evaluations  

---

## ✅ Next Steps  
Tomorrow (Day 11), you will create:  
✅ Security policies  
✅ Governance structure  
✅ Evidence library  
✅ Policy folder architecture  