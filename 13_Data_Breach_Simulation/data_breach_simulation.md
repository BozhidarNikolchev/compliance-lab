# Topic 13 – Data Breach Simulation
Author: Bozhidar Nikolchev  
Version: 1.0  
Last Updated: 2026‑03‑22  

---

## 1. Scenario Overview

### Incident Summary
At 03:14 UTC, the SIEM triggered a *Critical Alert* indicating unusual outbound data transfer from an application server (APP-SRV02). The traffic was directed to an unknown external IP belonging to a cloud storage provider. The transfer rate exceeded 3GB in under 15 minutes.

### Additional Indicators:
- A privileged service account (`svc-backend`) authenticated at 03:02 UTC from an IP address not previously used by that account.  
- EDR detected execution of a suspicious PowerShell script.  
- Web application logs show multiple failed login attempts followed by a successful login from the same IP.  
- Database access logs show large export queries (`SELECT * FROM users`) around the same time.

---

## 2. Assets Potentially Affected
- **APP-SRV02** (Windows Server) – backend application host  
- **User Database** – contains PII (emails, hashed passwords, profiles)  
- **Service Account `svc-backend`** – privileged access  
- **Outbound network filtering** – may have been bypassed  

---

## 3. Initial Assessment
Severity: **Critical**  
Reason:
- Possible personal data exfiltration  
- Privileged account compromise  
- Unusual outbound traffic  
- Multiple correlated suspicious events  

Regulatory Impact:  
- GDPR Article 33–34 may apply (potential PII breach)  

---

# 4. Step-by-Step Incident Response (Following Day 12 Procedures)

## 4.1 Identification
Actions:
- Validate SIEM alert and traffic logs.  
- Confirm unauthorized login to `svc-backend`.  
- Validate data export queries in DB logs.  
- Open Incident Ticket: **INC-2026-03-22-001**

---

## 4.2 Containment
Actions taken:
- Isolated APP-SRV02 from the network.  
- Disabled `svc-backend` credentials.  
- Blocked suspicious external IP at firewall.  
- Captured memory dump & forensic artifacts.

---

## 4.3 Eradication
Actions performed:
- Removed malicious PowerShell script.  
- Identified persistence mechanism in Scheduled Tasks — removed.  
- Patched vulnerable web component exploited for entry.  
- Rotated all privileged account passwords.

---

## 4.4 Recovery
Actions:
- Restored APP-SRV02 from clean backup.  
- Applied hardened configuration baseline.  
- Reconnected server after integrity validation.  
- Increased monitoring sensitivity for 72 hours.

---

## 4.5 Lessons Learned
- Root cause: Web API endpoint vulnerable to credential stuffing.  
- `svc-backend` lacked MFA (critical gap).  
- Outbound traffic monitoring was insufficient.  
- Database queries were not anomaly‑monitored.

Improvements required:
- Enforce MFA on ALL service accounts.  
- Implement data exfiltration detection rules.  
- Introduce rate limiting on login attempts.  
- Enhance DB monitoring (UEBA).

---

# 5. Evidence Collected
- SIEM alerts  
- Firewall logs  
- EDR telemetry  
- Memory dump (isolated offline)  
- Event logs showing unauthorized access  
- Database export logs  
- PowerShell script hash + copy  
- Timeline of attacker actions  

---

# 6. Data Breach Impact Summary
Data potentially exposed:
- Usernames  
- Emails  
- Hashed passwords  
- IP addresses  
- Registration metadata  

No financial data affected.  
No payment system touched.

Risk to individuals:
- Low likelihood of identity theft  
- Medium likelihood of targeted phishing  
- Medium reputational impact  

Regulatory report needed?
- **Yes**, under GDPR 33 (breach must be reported within 72 hours).

---

# 7. Breach Notification Plan
Internal notifications:
- Executives  
- Legal/Compliance  
- Data Protection Officer (DPO)  
- Engineering Lead

External notifications (if confirmed):
- Supervisory authority (within 72h)  
- Affected users (Article 34, if high risk to rights & freedoms)  

---

# 8. Final Breach Report Template (Portfolio Ready)  

Incident Title:
Incident ID:
Date Detected:
Reporting Analyst:
Severity Level:
Summary:
Provide a clear explanation of what occurred.
Affected Assets:
List systems, users, accounts, data types.
Impact Assessment:
Describe regulatory, business, and user impact.
Root Cause:
Explain how the breach happened.
Response Actions:
Containment:
Eradication:
Recovery:
Evidence Collected:
Notification Actions:
Corrective Actions:
Final Status:
Closed / Monitoring / Escalated

---

# 9. Framework Mapping

| Framework | Alignment |
|----------|-----------|
| ISO 27001 | A.5.24 / A.16 – Incident Management |
| NIST CSF | RS.AN, RS.MI, RS.CO – Detection & Response |
| PCI‑DSS | 12.10 – Incident Response Procedures |
| GDPR | Articles 33, 34 – Breach Notification |
| SOC 2 | CC7 – Incident Detection & Response |

---  

# 10. Completion Status
Day 13 completed.  
This file serves as the **official breach simulation documentation** for portfolio and training.

---  

## 📎 Exercise Files for Day 13

- [Scenarios Table- roles/role_assignments.md
- [Timeline Template](templates/timeline_template.md)
- [GDPR Article 33 Notification Formincident_report.md
- [Tabletop Simulation Worksheet](templates/tabletop_simulation_worksheet.md)  
