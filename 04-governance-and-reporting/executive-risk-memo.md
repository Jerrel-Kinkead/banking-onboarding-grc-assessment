# Executive Risk Memo: Digital Account Opening & IDV Launch

> **Disclaimer:** This memo is based on a simulated banking GRC portfolio scenario and fictional data.

* **To:** Chief Information Security Officer (CISO), Risk Committee, and VP of Digital Banking
* **From:** GRC / Risk Assessment Intern (Simulated Project)
* **Subject:** Pre-Launch Risk Summary & Remediation Priorities — VerifyFlow ID Integration
* **Date:** November 26, 2026

## 1. Purpose
This memo summarizes key cybersecurity, third-party, and data governance risks identified during the pre-launch assessment of **VerifyFlow ID**, the third-party identity verification (IDV) vendor supporting **Peachtree Community Bank's** online checking account onboarding flow.

## 2. Top Findings & Risk Summary
* **RSK-001 – Synthetic Identity & Spoofing Bypass (Inherent: 20 / High → Residual: 10 / Medium):** Fraudsters attempting to bypass online onboarding with synthetic identities or spoofing techniques pose high financial and KYC/AML exposure. Liveness checks, document tamper detection, velocity/device checks, and step-up review reduce residual risk, though ongoing tuning is needed during launch campaigns.
* **RSK-003 – Excessive Retention of Sensitive PII & Biometrics (Inherent: 15 / High → Residual: 6 / Low):** Storing ID scans, selfies/biometrics, and SSNs longer than required increases exposure under **GLBA Safeguards** and **NIST CSF 2.0 (`PR.DS`)** expectations. Enforcing clear retention/deletion schedules and encryption lowers residual risk.
* **RSK-002 & RSK-004 – Sub-Processor Oversight & API/Webhook Security (Inherent: 12 / Medium each):** Unapproved sub-processors (`GV.SC`) and weak API/webhook authentication (`PR.AA` / `PR.PT`) require contractual controls and technical verification prior to production traffic.
* **RSK-005 – Breach Notification SLA Clarity (Inherent: 10 / Medium → Residual: 5 / Low):** Ensuring clear, timely vendor incident notification (`GV.SC` / `RS.MA`) supports rapid bank response and regulatory readiness.

## 3. Recommended Pre-Launch Actions
1. **Verify API & Webhook Security Controls:** Confirm strong authentication, signed webhooks, and rate limiting before go-live (`RSK-004`).
2. **Lock In Data Retention & Sub-Processor Terms:** Confirm automated data deletion windows and approved sub-processor disclosures (`RSK-002`, `RSK-003`).
3. **Monitor Onboarding Fraud & Exceptions:** Track identity verification alerts, manual reviews, and incident escalations closely after launch (`RSK-001`, `RSK-005`).
