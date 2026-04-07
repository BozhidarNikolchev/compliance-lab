# Statement of Applicability (SoA) – ISO 27001:2022 (Simplified)
**Author:** Bozhidar Nikolchev  
**Day 7 Artifact – GRC / Compliance Analyst Portfolio**

---

## 1. Purpose
This Statement of Applicability (SoA) defines which ISO 27001:2022 Annex A controls are applicable to the organization, the justification for inclusion/exclusion, and the implementation/evidence status.

> This is a simplified portfolio version demonstrating your understanding of how a real SoA is structured.

---

## 2. Scope of the ISMS (Example)
The Information Security Management System (ISMS) covers all information systems, processes, and assets that handle, store, or process customer, employee, operational, and security‑sensitive data.

---

## 3. Risk Assessment Basis
Applicable controls are selected based on:
- Identified risks from the formal risk assessment
- Legal/regulatory requirements (GDPR, contractual, industry)
- Business requirements
- Third‑party/vendor dependencies

---

## 4. SoA Table (Sample Controls)
This is a **mini‑SoA** demonstrating the structure used in real ISO implementations.

| Control ID | Control Name | Applicable? | Justification | Implementation Status | Evidence |
|------------|--------------|-------------|---------------|------------------------|----------|
| A.5.1 | Information Security Policy | Yes | Required for governance and ISO certification | Implemented | Approved policy document |
| A.5.7 | Threat Intelligence | Yes | Needed to detect/prevent ransomware & emerging threats | Partially implemented | Threat reports; SOC integration |
| A.5.12 | Classification of Information | Yes | Protects sensitive and personal data | Implemented | Data classification policy |
| A.5.20 | Supplier Relationships Security | Yes | Third‑party risk management requirement | Implemented | Vendor risk assessments; DPAs |
| A.6.3 | Information Security Awareness | Yes | Reduces human‑related risk | Implemented | Training completion records |
| A.7.1 | Physical Security Perimeter | Yes | Protects on‑prem equipment | Partially implemented | Facility access logs |
| A.8.1 | User Endpoint Protection | Yes | Prevents data leakage & malware | Implemented | MDM baseline / EDR dashboard |
| A.8.9 | Configuration Management | Yes | Required to avoid misconfigurations | Implemented | Baseline configs; CIS scans |
| A.8.23 | Authentication | Yes | Authentication controls required for confidentiality | Implemented | MFA report |
| A.8.28 | Encryption | Yes | Protects data at rest & in transit | Implemented | Encryption reports |

---

## 5. Non‑Applicable Controls (Examples)
These entries demonstrate your reasoning skills.

| Control ID | Control Name | Not Applicable Because |
|------------|--------------|-------------------------|
| A.7.4 | Protection Against Environmental Threats | No on‑prem data centers are used (cloud‑only architecture) |
| A.7.9 | Secure Disposal or Reuse of Equipment | Org does not manage hardware lifecycle directly; managed service provider handles disposal |

---

## 6. Review & Approval Process
- SoA reviewed **annually** or after major changes (e.g., new tech stack, new vendors).
- Changes approved by: **CISO / Security Manager**.
- Versioning maintained for audit trail.

---

## 7. Notes for Reviewers
This simplified document demonstrates:
- Understanding of ISO 27001 control applicability logic
- Risk‑based selection of controls
- Awareness of evidence & implementation artefacts

A full SoA normally contains all **93 controls**, version history, ownership, and cross‑links to policies and risk register.
