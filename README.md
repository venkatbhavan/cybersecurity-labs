# DORA Case Study — Mainufer Bank AG (fictional)

A bank-wide assessment against the EU **Digital Operational Resilience Act (DORA, Regulation (EU) 2022/2554)** for a
fictional Frankfurt bank, with a technical deep dive on a new AI customer-support chatbot.

The bank, its suppliers and all business figures are **fictional**. The chatbot test results are **real lab results**
from my [LLM Security Proxy](https://github.com/venkatbhavan/llm-security-proxy).

## Files

| ID | File | DORA pillar | What it shows |
|----|------|-------------|---------------|
| DORA-01 | `DORA-01_Scope_Memo.pdf` | Applicability | Why DORA applies, 10 ICT systems, classification of 10 business functions (8 critical or important), proportionality, EU AI Act and GDPR overlap |
| DORA-02 | `DORA-02_ICT_Risk_Register.xlsx` | ICT risk management (Art. 5–15) | 16 risks scored 5×5, with controls, target risk, DORA articles and ISO/IEC 27001:2022 Annex A mapping |
| DORA-03 | `DORA-03_Incident_Playbook.pdf` | Incident reporting (Art. 17–23) | Major-incident test (RTS 2024/1772), 4 h / 24 h / 72 h / 1 month deadlines, three worked scenarios, sample initial notification |
| DORA-04 | `DORA-04_Testing_Programme.pdf` | Resilience testing (Art. 24–25), information sharing (Art. 45) | 2027 test plan for all systems, real AI chatbot attack results, findings tracker, threat bulletin |
| DORA-05 | `DORA-05_Register_of_Information.xlsx` | Third-party risk (Art. 28–30) | 11 ICT providers, Art. 30(2)/(3) clause check for the AI provider |
| DORA-05 | `DORA-05b_Third_Party_Note_Exit_Plan.pdf` | Third-party risk (Art. 28(8), 29) | AI provider contract gaps, tested exit plan, cloud concentration risk |
| DORA-06 | `DORA-06_Management_Summary.pdf` | All | Key figures, top five gaps, board decisions |

## Highlights

- **Function-first scoping:** systems and suppliers are in scope because of the business functions they support.
- **Borderline incident judgement:** a 1 h 45 min online banking outage is classified as major only because the
  client and reputational thresholds are both met (scenario B).
- **Real evidence for AI risk:** against Gemini, the model refused social engineering but forwarded a SQL injection
  into a tool. Only the proxy caught it. Model safety alone is not a control.
- **Third-party reality check:** the AI provider's standard terms meet 3 of 15 Art. 30 clauses.

## Related work

- [LLM Security Proxy](https://github.com/venkatbhavan/llm-security-proxy): the control used in the chatbot deep dive
- `02-grc-iso27001`: ISO/IEC 27001 and NIS2 case study (EventCraft)

*Student case study by Venkat Bhavan Tati. Not legal advice.*
