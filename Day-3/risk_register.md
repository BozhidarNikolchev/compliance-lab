# Compliance Risk Register

## Overview
This document tracks compliance risks, their ratings, mitigating controls, and ownership.

---

## Risk Table

### Risk #1 — GDPR Data Breach  
| ID | Risk Name | Category | Description | Likelihood | Impact | Rating | Existing Controls | Recommended Controls | Owner | Review Date |
|----|-----------|----------|-------------|------------|--------|--------|-------------------|----------------------|-------|-------------|
| 1  | GDPR data breach | Cyber/Data | A ransomware attack that encrypts files | High | High | Critical | MFA (FIDO2), EDR (CrowdStrike Falcon) | MFA (Okta FastPass), ASM (Palo Alto Cortex Xpanse) | Chief Information Security Officer (CISO) | 2026-03-12 |

---

### Risk #2 — Insider Threat  
| ID | Risk Name | Category | Description | Likelihood | Impact | Rating | Existing Controls | Recommended Controls | Owner | Review Date |
|----|-----------|----------|-------------|------------|--------|--------|-------------------|----------------------|-------|-------------|
| 2  | Insider Threat | Internal Breach | Negligent employee ignoring security policies for convenience | High | High | Critical | UEBA | Egress, Browser Isolation, Automated Labeling | Insider Threat Analyst | 2026-03-10 |

---

### Risk #3 — AML Regulatory Non-Compliance  
| ID | Risk Name | Category | Description | Likelihood | Impact | Rating | Existing Controls | Recommended Controls | Owner | Review Date |
|----|-----------|----------|-------------|------------|--------|--------|-------------------|----------------------|-------|-------------|
| 3 | AML regulatory non-compliance | Financial Crime & Regulatory Risk | A high-net-worth client, "Mr. Carpenter," attempts to deposit $900,000 cash into a corporate account, claiming it is from a yacht sale but provides no documentation. | Medium | High | Critical | pKYC (Encompass), AI Behavioral Monitoring (ThetaRay) | Workflow Blocking (account creation locked until Source of Wealth verified), Automated Sanctions Screening | MLRO | 2026-03-10 |

---

## Risk Rating Logic
- **Rating = Likelihood × Impact**
- Matrix:
  - High × High = Critical  
  - Medium × Medium = Medium  
  - Mixed = contextual assessment  

> **Note:** Ratings are calculated manually using the Risk Matrix.

---

## Example Entry

| ID | Risk Name | Category | Description | Likelihood | Impact | Rating | Existing Controls | Recommended Controls | Owner | Review Date |
|----|-----------|----------|-------------|------------|--------|--------|-------------------|----------------------|-------|-------------|
| 1  | GDPR Data Breach | Cyber/Data | Unauthorized exposure of PII | High | High | Critical | IAM, Encryption | MFA, DLP system | Compliance Lead | 2026-03-01 |

---

## Version History
- v1.1 — Cleaned tables, removed auto-calc rows  
- v1.0 — Initial creation (Day 3)