# 04 Risk and obligations

## Risk class and human in the loop

- A report can end in a fine: it touches third parties' money and is hard to reverse.
- High risk → **human in the loop is mandatory**. It's already in the design: I review every report before it is sent.
- Triggers that keep a case out of review: low confidence, unreadable plate, unclear violation.

## Obligations: identify → map → evidence

**Identify** (they follow the reporting process, not the model):
- [ ] Traffic rules and the city's requirements for accepting citizen reports.

### Reporting channel (researched 2026-11-11)

| Channel | Video | Tracking | Covers other drivers' violations? |
|---|---|---|---|
| Montevideo SUR (Sistema Único de Respuesta), web form | Yes: photos, videos, PDF | Yes: email with follow-up link, closure notice | **Unconfirmed**: listed topics are cleaning, lighting, streets, sidewalks, transport |
| Montevideo 1950 4000 option 1 (traffic center) | No, phone only | Not stated | Yes, but aimed at urgent cases |
| Montevideo WhatsApp 099 019 500 | Not stated for reports | Not stated | Not stated: listed for inquiries, fines and noisy exhausts |
| Canelones | No channel found (app for local problems, 1828 phone line) | — | — |

- Candidate: **SUR**, because it is the only channel with both video and a tracking record (needed for the lagging KPI).
- SUR asks for a captcha at the start. The captcha comes first, so the agent can't even pre-fill the form. Control: the agent leaves each report in a "ready to send" folder (clip + text per field); **I fill in SUR by hand, solve the captcha and send**. The agent never touches the form and nothing tries to bypass the captcha.
- [ ] Open: does SUR have a category that fits a traffic violation by another driver? Check step 2 of the form, then send one real test report.
- [ ] Data protection: plates and faces of third parties who did nothing get filmed.
- AI requirements on top: explain each report, a review route, recorded evidence.

**Map** (one control per obligation):
- Mask faces and plates that aren't the offender's.
- Retention: delete clips with no violation.
- A reason per report: clip + rule broken.

**Evidence** (logged from day one):
- Per report: clip, rule, model version, who reviewed it and when.
