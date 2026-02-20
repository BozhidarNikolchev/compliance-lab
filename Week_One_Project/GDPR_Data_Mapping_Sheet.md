# GDPR Data Mapping Sheet — Inventory & Flow Mapping
**Author:** Bozhidar Nikolchev
**Version:** 1.0  
**Last Updated:** 2026‑02‑20  

---

## 📘 How to Use
Use this sheet to document all systems that store or process personal data.  
Add one row per dataset or system.

---

## 1. System Inventory
| System | Data Categories | Purpose | Lifecycle Stage | Legal Basis | Storage Location | Risk Level | Owner |
|--------|-----------------|----------|------------------|-------------|-------------------|------------|--------|
| CRM | Name, email | Customer management | Collection → Storage | Contract | EU Cloud | Medium | Sales |
| Website Analytics | IP, device info | Usage analytics | Monitoring | Legitimate interest | US Cloud | High | Marketing |

---

## 2. Data Flow Description
Example:
Form submission → Web server → CRM → Support team → Archived after 24 months

---

## 3. Retention Schedule
| Data Category | Retention | Disposal Method |
|----------------|-----------|------------------|
| Account data | 3 years | Secure deletion |
| Logs | 12 months | Automated purge |

---

## 4. Third‑Party Processors
| Vendor | Purpose | Region | Safeguards |
|--------|----------|--------|--------------|
| Stripe | Payments | EU/US | SCCs |
| Google Analytics | Analytics | US | SCCs |

---

## 5. Risk Flags
- ☐ Missing DPA  
- ☐ High-risk data  
- ☐ International transfers  
- ☐ Sensitive data involved  