# Topic 1 — Compliance Theory Notes

## GDPR

### What it is
GDPR stands for the General Data Protection Regulation, a comprehensive EU privacy law that took effect on May 25, 2018.

### Why it exists
It is widely considered the strongest privacy and security law in the world, designed to give individuals more control over their personal data and ensure organizations process data responsibly.

### The 7 principles
Organizations must follow seven key principles:
1. Lawfulness, fairness, and transparency  
2. Purpose limitation  
3. Data minimization  
4. Accuracy  
5. Storage limitation  
6. Integrity and confidentiality  
7. Accountability

### Rights of data subjects
GDPR grants eight fundamental rights:
- Right to be informed  
- Right of access  
- Right to rectification  
- Right to erasure (“right to be forgotten”)  
- Right to restrict processing  
- Right to data portability  
- Right to object  
- Rights around automated decision‑making and profiling

### Key obligations for companies
Companies must implement:
- Lawful bases for processing  
- Strong security controls  
- Transparent privacy notices  
- Data breach reporting  
- Risk management and documentation (DPIAs, RoPA)  
- Accountability through policies, audits, and training

---

## Global Privacy Laws

### USA
- No single federal privacy law  
- Sector‑specific laws (HIPAA, GLBA, COPPA)  
- Increasing number of state‑level comprehensive laws (e.g., CCPA/CPRA)

### China (PIPL)
- Enacted 2021  
- One of the strictest privacy laws globally  
- GDPR‑like requirements with strong enforcement and consent rules

### India (DPDP Act)
- Enacted August 2023  
- India’s first comprehensive privacy framework  
- Introduces consent, data rights, and obligations for data fiduciaries

---

## AML & KYC

### What KYC is
KYC (Know Your Customer) is the mandatory process used to verify customer identity and prevent fraud, money laundering, and terrorist financing.

### What AML is
AML (Anti‑Money Laundering) is the broader regulatory framework designed to:
- Prevent illegal funds from entering the financial system  
- Detect suspicious transactions  
- Ensure reporting to authorities  
Modern AML (2026) includes **real‑time monitoring** and **perpetual KYC**.

---

### CIP / CDD / EDD

#### CIP (Customer Identification Program)
**Purpose:** Verify that the person is who they claim to be.  
**Minimum required data:**  
- Name  
- Date of Birth  
- Address  
- Identification Number (SSN, passport, etc.)  
**Actions:**  
- ID verification  
- Liveness/biometric checks  

#### CDD (Customer Due Diligence)
**Purpose:** Understand the customer profile and expected behavior.  
**Actions:**  
- Identify the UBO (for businesses)  
- Determine purpose of account  
- Sanctions, PEP, and adverse media screening  

#### EDD (Enhanced Due Diligence)
Triggered by high-risk customers (PEPs, high‑risk jurisdictions, unusual patterns).  
**Actions:**  
- Source of Wealth (SoW)  
- Source of Funds (SoF)  
- More frequent reviews (quarterly)

---

### Sanctions & PEP Screening

#### Sanctions Screening
- Mandatory for all financial institutions  
- Screen against OFAC, EU Restrictive Measures, UN Lists, etc.  
- Uses fuzzy matching to detect name variations  
- Strict liability: even $1 processed for a sanctioned entity = violation

#### PEP Screening
- PEP = person with political influence or exposure  
- Includes RCA (Relatives and Close Associates)  
- Not forbidden — but *always high-risk* → triggers EDD  
- Usually requires senior management approval

### Why these matter
GDPR, AML, KYC, sanctions, and PEP screening form the **frontline defense** against financial crime, fraud, corruption, and data misuse.

---

## PCI DSS

### What PCI DSS is
A global security standard ensuring that companies handling credit card data protect that data effectively.

### Who must comply
Any organization (any size) that:
- Stores  
- Processes  
- Transmits  
cardholder data.

### PCI DSS 4.0 key changes
- Stronger Multi‑Factor Authentication  
- Better protections against e‑commerce attacks (Magecart)  
- “Customized Approach” for flexibility  
- Stronger cryptography standards  
- Increased review/testing frequency  

### The 12 requirements (summary)
1. Network security controls (firewalls/NSCs)  
2. Secure system configurations  
3. Protect stored account data  
4. Encrypt data during transmission  
5. Protect systems from malware  
6. Patch and maintain secure systems  
7. Restrict access by business need  
8. Identify and authenticate access  
9. Restrict physical access  
10. Log and monitor all access  
11. Regular security testing  
12. Maintain a security policy and training  

---

## ISO 27001

### What an ISMS is
An ISMS (Information Security Management System) is a structured set of policies, procedures, and controls used to secure information and reduce organizational risk.

### Why ISO matters
As of October 2025, ISO/IEC 27001:2022 certification is required to maintain compliance.  
It demonstrates:
- Strong security maturity  
- Risk-based governance  
- International trustworthiness  

### ISO/IEC 27001:2022 updates
Key changes include:
- Modernized, risk-based controls  
- Focus on cybersecurity and cloud security  
- Annex A controls reduced from 114 → 93  
- 11 new controls (threat intelligence, secure coding, cloud services, etc.)