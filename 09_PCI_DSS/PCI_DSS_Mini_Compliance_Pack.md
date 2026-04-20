# PCI-DSS Mini Compliance Pack

**Author:** Bozhidar Nikolchev  
**Date:** 2026-03-17  
**Program:** Topic 9 – PCI-DSS Mini Compliance Pack

---

## Contents

- `pci_dss_controls.csv` — PCI-DSS requirements and sub-controls list.

- `pci_dss_gap_assessment_template.csv` — Ready-to-use gap assessment sheet.


## How to Use

1. Start with **pci_dss_gap_assessment_template.csv** and fill `Current State`, `Evidence`, `Owner`, and `Due Date`.

2. Rate risk and set priorities (P1=urgent, P2=important, P3=nice-to-have).

3. Track remediation status until all gaps are Closed.

4. Keep evidence links (tickets, change records, screenshots) for auditability.


## Scope Assumptions

- Cardholder Data Environment (CDE) with segmented network.

- TLS 1.2+ for all public transmissions.

- PAN rendered unreadable at rest (tokenization or encryption).


## Evidence Examples

- Network diagram, firewall rule exports, segmentation test results.

- Key management SOPs and HSM configs.

- SIEM dashboards, log retention policy, daily review records.

- Quarterly ASV reports, annual pentest report, remediation tickets.


## Risk Scenarios (sample)

- **Unencrypted PAN in logs** → data exposure → regulatory fines and reputation loss.

- **Expired TLS certificate** → MITM risk during checkout → transaction failures.

- **No MFA for admin access** → credential stuffing → CDE compromise.

- **Weak firewall egress rules** → data exfiltration via outbound channels.


## Mapping Tips

- Link Req. 5/6 to vulnerability management SLOs (patch windows).

- Align Req. 10 with centralized logging and 12-month retention.

- Connect Req. 12 to policy lifecycle, training, and vendor risk.
