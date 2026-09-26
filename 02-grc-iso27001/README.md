# GRC & ISO/IEC 27001 — EventCraft Risk Assessment

Self-directed application of ISO/IEC 27001 risk management and NIS2 regulatory
scoping to a real system: EventCraft, the role-based event management platform
built as part of the Master Team Project (GDSD program, Hochschule Fulda).

## Contents

- **`EventCraft_ISO27001_Risk_Register.xlsx`** — a 14-item risk register scored
  against EventCraft's actual documented architecture (Azure VM, MySQL, JWT
  auth, file uploads, Socket.IO chat, RBAC, third-party AI integration,
  CI/CD, QR check-in tokens). Uses a 5×5 Likelihood × Impact matrix per
  ISO/IEC 27005 practice referenced in ISO/IEC 27001 Clause 6.1.2. Items
  without independently verified evidence are explicitly marked
  "Unverified" or "Not documented" rather than assumed.
- **`EventCraft_NIS2_Applicability_Note.docx`** — a worked analysis of
  whether a platform like EventCraft would fall under the EU's NIS2
  Directive if operated commercially, applying the actual sector + size
  scoping test, and mapping all 10 categories of NIS2 Article 21(2)
  measures back to specific rows in the Risk Register.

## Methodology

Risks were identified from the platform's documented data entities,
authentication/authorization design, and known architectural decisions.
Existing controls are drawn from the actual implementation where
documented — this is not a generic template applied to a fictional
company; it's a real assessment of a real (student) system, done honestly,
gaps included.

## Status

Risk R-07 (admin/RBAC privilege escalation) is currently marked
"Unverified" pending a hands-on access-control test — see
[`01-web-application-pentesting`](../01-web-application-pentesting) for
related findings as they're documented.

## Author

Prepared by Venkat Bhavan Tati as an independent learning exercise —
not an official audit of EventCraft or an endorsement by the EventCraft
project team.
