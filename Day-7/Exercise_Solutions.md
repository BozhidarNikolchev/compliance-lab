
# Day 7 Exercise – Sample Solutions (Risk → Control)
**Author:** Bozhidar Nikolchev  

Below are three fully worked examples you can adapt.

---

## Risk: Misconfigured Cloud Storage (Public S3 Bucket)
**Relevant ISO Controls**  
- A.8.9 Configuration management  
- A.8.28 Encryption  
- A.5.7 Threat intelligence  

**Implementation**  
- Organization‑wide bucket policies denying public ACLs  
- Server‑side encryption by default (SSE‑S3/KMS)  
- Continuous misconfiguration scanning (e.g., CSPM)  

**Evidence**  
- Policy JSON exports  
- KMS key policy screenshots  
- CSPM report showing zero public buckets

---

## Risk: Third‑Party Vendor Breach (Data Processor)
**Relevant ISO Controls**  
- A.5.20 Supplier relationships security  
- A.5.19 Information security in project management  
- A.8.15 Logging and monitoring  

**Implementation**  
- Security addendum and DPA with minimum control set  
- Pre‑contract security questionnaire and risk rating  
- Contractual right‑to‑audit; log shipping from vendor where applicable  

**Evidence**  
- Signed DPA and security schedule  
- Completed vendor risk assessment  
- Audit/pen test reports or SOC 2 from vendor

---

## Risk: Lost or Stolen Laptop
**Relevant ISO Controls**  
- A.8.1 User endpoint protection  
- A.8.28 Encryption  
- A.6.3 Awareness  

**Implementation**  
- Full‑disk encryption with escrowed recovery keys  
- Automatic lockout and remote wipe via MDM  
- User training on reporting lost devices within 24 hours  

**Evidence**  
- Encryption status report  
- MDM wipe logs and incident record  
- Training acknowledgement