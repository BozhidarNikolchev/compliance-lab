# Vendor Inventory

This document lists all third‑party vendors used by the organization.  
Each vendor is classified by criticality based on data processed, business impact,
and operational dependency.

| Vendor            | Service Provided            | Data Processed                | Criticality | Notes                                 |
|------------------|-----------------------------|-------------------------------|-------------|----------------------------------------|
| Microsoft 365     | Email + document storage    | Personal + internal data      | Tier 1      | Core communication platform             |
| AWS               | Cloud hosting + compute     | Operational + customer data   | Tier 1      | EU region required                      |
| Trello            | Task & project management   | Minimal personal data         | Tier 3      | Used by Marketing                       |
| HubSpot           | CRM + marketing automation  | Contact data (PII)            | Tier 2      | Must review DPA + sub-processor list    |
| Slack             | Internal communication      | Internal operational data     | Tier 2      | Optional Enterprise Key Management      |