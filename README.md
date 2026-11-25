# Banking Onboarding & IDV GRC Risk Assessment

> **Disclaimer:** This organization, vendor, and risk assessment are fictional/simulated for an entry-level Governance, Risk, and Compliance (GRC) portfolio project.

## Overview
This repository presents a simulated third-party risk and compliance assessment for **Peachtree Community Bank** as it launches an online deposit account opening flow integrated with a third-party Identity Verification (IDV) and KYC vendor (**VerifyFlow ID**).

Because digital onboarding processes sensitive customer information—including government IDs, selfies/biometrics, Social Security Numbers (SSNs), dates of birth, and device/IP metadata—this project focuses on identifying key risks, scoring inherent versus residual exposure, and mapping controls to banking-relevant guidance.

## Frameworks & Regulatory Concepts Referenced
* **NIST Cybersecurity Framework (CSF) 2.0:** *Govern* (`GV.SC`), *Protect* (`PR.AA`, `PR.DS`, `PR.PT`), *Detect* (`DE.CM`), and *Respond* (`RS.MA`).
* **GLBA Safeguards Rule Concepts:** Risk assessment, data protection and retention discipline, access controls, and oversight of third-party service providers.

## Repository Contents
* **Vendor Due Diligence (`vendor-profile.md`):** Banking context, Tier 1 vendor criticality rationale, data flows, and regulatory alignment.
* **Risk Register (`03-risk-register/onboarding-idv-risk-register.csv`):** Five simulated risks (`RSK-001` through `RSK-005`) scored on a 1–5 Likelihood × 1–5 Impact scale with mitigating controls, residual scores, treatments, owners, and target dates.

## Planned Next Additions
* NIST CSF 2.0 control gap analysis with required audit evidence
* 1-page executive risk memo for leadership/risk committee review
