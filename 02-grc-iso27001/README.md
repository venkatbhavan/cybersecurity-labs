# GRC & ISO/IEC 27001 — EventCraft Risk Assessment

Self-directed application of ISO/IEC 27001 risk management and NIS2 regulatory scoping to a real system: **EventCraft**, the role-based event management platform built as part of the Master Team Project (GDSD program, Hochschule Fulda).

## Contents

| Document | View | Source |
|---|---|---|
| **ISO/IEC 27001 Risk Register (v2)** | [PDF](EventCraft_ISO27001_Risk_Register.pdf) | [Excel](EventCraft_ISO27001_Risk_Register.xlsx) |
| **NIS2 Applicability Note** | [PDF](EventCraft_NIS2_Applicability_Note.pdf) | [Word](EventCraft_NIS2_Applicability_Note.docx) |

- **Risk Register:** 14 risks scored against EventCraft's actual documented architecture (Azure VM, MySQL, JWT auth, file uploads, Socket.IO chat, RBAC, third-party AI integration, CI/CD, QR check-in tokens). It uses a 5×5 Likelihood × Impact matrix per ISO/IEC 27005 practice referenced in ISO/IEC 27001 Clause 6.1.2. Each risk carries its existing controls, treatment option (Mitigate / Accept), treatment plan, target residual risk, **ISO/IEC 27001:2022 Annex A controls** and the **evidence basis** for its rating.
- **NIS2 Applicability Note:** a worked analysis of whether a platform like EventCraft would fall under the EU's NIS2 Directive if operated commercially, applying the sector + size scoping test, including Germany's transposition (NIS2UmsuCG, in force since 6 December 2025), and mapping all 10 categories of NIS2 Article 21(2) measures back to specific rows in the Risk Register.

## Methodology

Risks were identified from the platform's documented data entities, authentication/authorization design and known architectural decisions. Existing controls are drawn from the actual implementation where documented. This is not a generic template applied to a fictional company; it's a real assessment of a real (student) system, done honestly, gaps included.

**Risk Score** is the current risk with existing controls in place. **Target Residual Risk** is the expected level after the treatment plan, so it never exceeds the current risk. Items without independently verified evidence are explicitly marked "Unverified" or "Not documented" rather than assumed.

## Version history

- **v1 (Sep 2026):** initial assessment based on architecture documentation.
- **v2 (Nov 2026):** hands-on testing confirmed **insecure file upload (R-05)**, **prompt injection in the AI integration (R-08)**, and **SQL injection and stored XSS (R-10)**. These three risks were re-rated (two now High, one Medium) and set to *Open — confirmed by testing*, which shows that controls documented in the architecture were incomplete in practice. Also added: Annex A control mapping, treatment options, evidence basis, a consistent residual-risk definition, and the German NIS2 transposition.

## Status

- **3 risks confirmed by testing** (R-05, R-08, R-10): open, with re-test after remediation.
- **R-07** (admin/RBAC privilege escalation) remains *Unverified* pending a hands-on access-control test.
- A write-up of the EventCraft web application testing is in preparation; methodology examples are in [01-web-application-pentesting](../01-web-application-pentesting).

## Author

Prepared by Venkat Bhavan Tati as an independent learning exercise, not an official audit of EventCraft or an endorsement by the EventCraft project team.
