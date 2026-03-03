

<!--
Title: Incident Runbook – RS
Author: Bozhidar Nikolchev  
Program: 30-Day Compliance – Day 8 (NIST CSF)
Date: 2026-03-03
-->


# Incident Runbook – Respond (RS)

**Trigger**: High-severity incident detected (SIEM/EDR/IR channel).
**Steps**:
1. **Triage** (DE.AE) – categorize & prioritize (SEV1-4)
2. **Contain** (RS.MI) – isolate affected hosts/accounts
3. **Eradicate** – remove root cause, patch, reset credentials
4. **Recover** (RC.RP) – restore and validate
5. **Communicate** (RS.CO) – notify stakeholders
6. **RCA & Lessons Learned** (RS.AN, ID.IM)
**RACI**: IR Lead (A), SOC (R), IT Ops (R/C), Legal (C), Comms (C), Exec (I)
