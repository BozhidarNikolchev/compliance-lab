# Incident Response Procedures
Author: Bozhidar Nikolchev  
Version: 1.0  
Status: Draft  
Last Updated: 2026‑03‑22  

---

## 1. Purpose
These Incident Response Procedures provide a structured, repeatable, and efficient process for detecting, analyzing, containing, eradicating, and recovering from security incidents.  
They support the Incident Response Policy and ensure alignment with ISO 27001, NIST CSF, SOC 2, PCI‑DSS, and GDPR.

---

## 2. Scope
These procedures apply to:

- All security incidents and suspected incidents  
- All employees, contractors, and third parties  
- All IT systems, cloud services, networks, and applications  

---

# 3. Incident Severity Classification Matrix

| Severity | Description | Examples | Required Response Time |
|----------|-------------|----------|-------------------------|
| **Low** | Minor event, no impact | Failed login attempts, phishing email blocked | 24–48 hours |
| **Medium** | Potential security risk | Malware detected and quarantined, suspicious login | 12–24 hours |
| **High** | Confirmed incident affecting systems | Unauthorized access, data leakage attempt | 1–4 hours |
| **Critical** | Major incident with business or regulatory impact | Active breach, ransomware, confirmed data exfiltration | Immediate (0–1 hour) |

---

# 4. Incident Response Lifecycle (Operational Steps)

## 4.1 Preparation
- Ensure monitoring, alerting, and logging systems are functioning.  
- Maintain up‑to‑date escalation contacts and IRT roster.  
- Verify that IR tools (SIEM, EDR, forensic tools) are available and accessible.

---

## 4.2 Identification
**Goal:** Detect and confirm the incident.

Steps:
1. Receive alert from SIEM/EDR, monitoring tools, or employee report.  
2. Validate alert legitimacy.  
3. Classify severity based on matrix.  
4. Open an Incident Ticket (format in Section 8).  
5. Notify stakeholders per Communication Plan.

---

## 4.3 Containment
**Goal:** Limit damage before it spreads.

Short‑term containment:
- Isolate affected endpoints (EDR quarantine).  
- Disable compromised user accounts.  
- Block malicious IPs/domains.  
- Remove system from the network if necessary.

Long‑term containment:
- Apply temporary firewall rules.  
- Patch the vulnerable system.  
- Reset credentials or API keys.

---

## 4.4 Eradication
**Goal:** Remove the threat completely.

Steps:
- Remove malicious files or scripts.  
- Clean infected systems.  
- Terminate unauthorized processes or sessions.  
- Apply patches or configuration fixes that eliminate root cause.

---

## 4.5 Recovery
**Goal:** Restore services securely.

Steps:
- Restore systems from clean backups.  
- Reconnect system to network after validation.  
- Monitor logs for recurring suspicious activity.  
- Verify business functionality.

---

## 4.6 Lessons Learned
Must be conducted **within 7–14 days** of incident closure.

Deliverables:
- Root Cause Analysis (RCA)  
- Timeline of events  
- Actions performed and by whom  
- Control improvements required  
- Updated documentation, policies, or procedures  

---

# 5. Roles and Responsibilities (Operational Layer)

### Incident Response Team (IRT)
- Leads investigations  
- Performs containment, eradication, and recovery  
- Documents all actions in the incident ticket  

### IT Operations
- Applies patches  
- Restores systems  
- Provides logs and technical assistance  

### Security/GRC Lead
- Coordinates communication  
- Ensures regulatory reporting compliance  

### Executive Management
- Approves major decisions for high/critical incidents  

### All Employees
- Report incidents immediately  
- Cooperate with investigators  

---

# 6. Communication & Escalation Plan

### When to escalate:
- **High severity** = notify IT, Security, and Management  
- **Critical severity** = notify Executives immediately

### Communication channels:
- Incident hotline  
- Email alert group  
- Messaging channel (#incident‑response)  
- Ticketing system (JIRA/ServiceNow)  

### External communication:
- Legal/compliance for GDPR 72‑hour breach reporting  
- Vendors if third‑party systems are affected  
- Customers if required by contract  

---

# 7. Evidence Collection Checklist
The following evidence must be collected and preserved:

- System logs (Windows Event Logs, Linux Syslog)  
- Network traffic (pcap, firewall logs)  
- EDR telemetry  
- Screenshots of unusual activity  
- User session history  
- File hashes and timestamps  
- Access logs and failed login attempts  

All evidence must follow chain‑of‑custody procedures.

---

# 8. Incident Ticket Template  

Incident Title:
Incident ID:
Severity Level:
Date/Time Detected:
Detected By:
Systems Affected:
Summary:
Indicators of Compromise (IOCs):
Containment Actions Taken:
Eradication Steps:
Recovery Notes:
Evidence Collected:
Root Cause Analysis:
Lessons Learned:
Status:  

---

# 9. Framework Mapping

| Framework | Requirement |
|----------|-------------|
| ISO 27001 | A.5.24, A.16 – Incident Management |
| NIST CSF | RS.* – Respond Function |
| PCI‑DSS | 12.10 – Incident Response Plan |
| GDPR | Article 33–34 – Breach Notification |
| SOC 2 | CC7 – Monitoring & Incident Response |

---

# 10. Review and Maintenance
These procedures must be reviewed:

- Annually  
- After major incidents  
- When systems or roles change  
- When regulatory requirements change  

---  