# 02 Baseline and KPIs

## Claim vs evidence

> "There are many more violations in Montevideo than in Canelones."

Today this is a **claim, not evidence**: there is no comparable record.

To become evidence, the baseline has to pass the three checks:

1. **Recorded before** anything is built.
2. **Same measurement:** violations per hour driven (not just a count, because time spent in each area differs).
3. **Comparable period:** same time slot and type of day when comparing areas.

## Triage baseline (ASSUMED, practice data)

> **Mock numbers, not evidence.** Made up to work the case. They have to be replaced by one real SD session before the gate to experiment.

One monthly SD session today:

| Step | Volume | Time |
|---|---|---|
| Clips on the card (button + automatic G-sensor events) | ~120 | — |
| Watch each clip and decide | ~1.5 min per clip | ~3 h |
| Real violations found | ~30 (25%) | — |
| Clips that need cutting or converting | ~20 of 30, ~3 min each | ~1 h |
| **Triage total** | | **~4 h** |
| Fill in the form (fixed, out of scope) | ~3 min per report | ~1.5 h |
| Delay from violation to report | up to ~30 days | — |

Target: triage under 30 minutes (≈ 30 ready candidates × ~1 min to approve or drop).

## KPIs

| Type | KPI | When |
|---|---|---|
| Leading | Triage minutes per monthly session (the outcome) | months 1 to 3 |
| Leading | % of candidates I approve on review (precision) | months 1 to 3 |
| Leading | Real violations the model missed, from a sample I check by hand (recall) | months 1 to 3 |
| Leading | % of approved clips that need no further editing | months 1 to 3 |
| Lagging | Reports accepted per month (quality guardrail) | later |
| Lagging | % of sent reports the city accepts (quality guardrail) | later |

## Costs

- **Build:** training or adapting the model, clip-cutting pipeline. In-car hardware only if real time turns out to be needed.
- **Run:** compute per monthly batch, agent usage, review minutes.

## Public totals

Updated from `private/log.md`.

| Area | Hours driven | Violations | Per hour |
|---|---|---|---|
| Montevideo | - | - | - |
| Canelones | - | - | - |
