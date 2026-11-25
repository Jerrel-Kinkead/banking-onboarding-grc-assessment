# Vendor Profile: Digital Account Opening & Identity Verification (IDV)

> **Disclaimer:** This organization, vendor, and risk assessment are fictional/simulated for an entry-level banking GRC portfolio project.

## 1. Banking Context & Product Scope
**Peachtree Community Bank** (simulated regional bank) is launching an online deposit account opening flow that allows prospective customers to apply for checking accounts digitally. To support Know Your Customer (KYC) and identity verification requirements, the bank integrates with a third-party Identity Verification & Document Authentication vendor (**VerifyFlow ID**, simulated).

## 2. Vendor Tiering & Criticality
* **Assigned Tier:** Tier 1 – Critical Vendor
* **Rationale:** The service processes high-sensitivity customer Personally Identifiable Information (PII) and identity verification data, supports core customer onboarding availability, and presents elevated fraud and regulatory exposure if compromised or unavailable.

## 3. Data Flows & Sensitive Information Handled
* **Data Collected/Processed:** Government-issued ID images, selfies/liveness check captures, Social Security Numbers (SSNs), dates of birth, residential addresses, email/phone contact details, and device/IP metadata.
* **Data Transmission & Storage:** Applicant data is submitted via encrypted APIs during onboarding, evaluated by the vendor's verification service, and returned to the bank via status callbacks/webhooks along with verification outcomes and audit metadata.

## 4. Regulatory & Framework Alignment
* **NIST Cybersecurity Framework (CSF) 2.0:** Informed by **Govern** (`GV.SC` Cybersecurity Supply Chain Risk Management), **Protect** (`PR.AA` Identity Management, Authentication, and Access Control; `PR.DS` Data Security), **Detect** (`DE.CM` Continuous Monitoring), and **Respond** (`RS.MA` Incident Management).
* **GLBA Safeguards Rule Concepts:** Aligns with risk assessment, data protection/encryption, access safeguards, data disposal/retention discipline, and ongoing oversight of service providers handling customer information.

## 5. Key Risks Linked to This Vendor
See `03-risk-register/onboarding-idv-risk-register.csv` for detailed scoring and treatments (`RSK-001` through `RSK-005`), including synthetic identity/spoofing bypass, sub-processor transparency, data retention limits, API/webhook authentication, and breach notification SLAs.
