# 04 Risk and obligations

## Risk class and human in the loop

- A report can end in a fine: it touches third parties' money and is hard to reverse.
- High risk → **human in the loop is mandatory**. It's already in the design: I review every report before it is sent.
- Triggers that keep a case out of review: low confidence, unreadable plate, unclear violation.

## Obligations: identify → map → evidence

**Identify** (they follow the reporting process, not the model):
- [ ] Traffic rules and the city's requirements for accepting citizen reports.
- [ ] Data protection: plates and faces of third parties who did nothing get filmed.
- AI requirements on top: explain each report, a review route, recorded evidence.

**Map** (one control per obligation):
- Mask faces and plates that aren't the offender's.
- Retention: delete clips with no violation.
- A reason per report: clip + rule broken.

**Evidence** (logged from day one):
- Per report: clip, rule, model version, who reviewed it and when.
