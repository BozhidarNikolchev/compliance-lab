
# Vendor Risk Assessment — HubSpot (Day 15 VRM)

## 1. Executive Summary
HubSpot is a global CRM and marketing automation platform with strong security maturity. Its security posture includes SOC 2 Type II, SOC 3, GDPR compliance, annual penetration testing, and globally distributed, secure data centers. Overall risk: **Medium-Low**.

## 2. Vendor Information
- **Vendor:** HubSpot
- **Founded:** 2006 (Source: HubSpot Trust Center)
- **Service:** CRM, marketing automation, customer engagement
- **Hosting:** Global data centers in EU, Canada, Australia, US East & West
- **Trust Center:** Provides SOC reports, security documentation, sub-processor lists

## 3. Certifications & Compliance
- SOC 2 Type II
- SOC 3
- HIPAA, GDPR, CCPA, EU Cloud Code of Conduct
- Annual third-party audits
- Annual penetration testing

## 4. Infrastructure & Data Centers
HubSpot operates multiple global data centers with:
- Advanced physical security
- 24/7 monitoring
- Redundant power and cooling
- Disaster recovery systems
- Regular audits and infrastructure updates

## 5. Technical Security Controls
### Encryption
- TLS 1.2+ in transit
- TLS enabled by default
- 2048-bit or better encryption

### Network & Application Security
- Web Application Firewall
- Network-level firewalls
- DDoS protection
- Secure SDLC with static code analysis

### Vulnerability Management
- Recurring penetration tests
- Regular vulnerability scanning
- Patch management program

### Incident Response
- Documented IR procedures
- Regular response exercises

## 6. Privacy & GDPR Evaluation
- Full Data Processing Agreement (updated 2026)
- SCCs for international transfers
- Sub-processor list available
- European data provisions included

## 7. Operational Controls
- Documented business continuity plan
- Redundant infrastructure
- Monitoring and intrusion detection

## 8. March 12, 2026 Security Advisory
HubSpot identified a phishing campaign targeting customers and took immediate remedial action, demonstrating strong transparency and mature incident response.

## 9. Risk Scoring
| Category | Score |
|----------|--------|
| Confidentiality | Medium |
| Integrity | Low |
| Availability | Low |
| Compliance Risk | Low |
| **Overall Risk** | **Medium-Low** |

## 10. Recommendation
✅ **Approved** with annual review
✅ Tier classification: **Tier 2** (Tier 1 if storing customer PII)
✅ Requires DPA and sub-processor review
