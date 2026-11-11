<div align="center">

# Dashcam traffic violations, by the book

[![Framework](assets/badges/framework.svg)](#the-brief)
[![Stage](assets/badges/stage.svg)](#the-board)
[![Blocking gaps](assets/badges/blocking.svg)](#the-board)
[![Raw data](assets/badges/privacy.svg)](#privacy)
[![License](assets/badges/license.svg)](LICENSE)

### An AI idea taken through the AIB-C01 framework before a single line of code.

A dashcam spots traffic violations, an agent drafts the report, a person reviews it<br>
and sends it to the city. This repo is the business case, not the build.

</div>

---

## The brief

I report traffic violations by hand: press the dashcam button, save the clip, file it. It happens every day. The idea is to let a small model in the car spot them, an agent draft the report and keep me as the reviewer before anything is sent.

Instead of starting with the hardware, this repo runs the idea through what the [AWS Certified AI Business Strategist](https://github.com/Barralex/aws-ai-business-strategist) exam teaches: outcome first, rules or AI, build or buy, a credible baseline, risk and obligations, bias, monitoring, maturity and readiness gaps. Each question I can't answer yet becomes an open gap on the board.

**Outcome:** the city receives reports of real violations, with evidence it can act on.

## The board

The weakest dimension decides, not the average.

| Piece | Status | Open gap |
|---|---|---|
| [Outcome and use case](01-outcome-y-use-case.md) | 🟡 | Target reports per month not set |
| [Baseline and KPIs](02-baseline-y-kpis.md) | 🔴 | "Montevideo has more" is a claim, not evidence |
| [Risk and obligations](04-riesgo-y-obligaciones.md) | 🔴 | Does the city accept citizen reports with video? |
| [Bias and monitoring](05-bias-y-monitoreo.md) | 🟡 | No per-group measure defined |
| [Leadership alignment](06-madurez-y-gaps.md) | 🟡 | I am sponsor and owner at once |
| [Data quality](06-madurez-y-gaps.md) | 🔴 | Manual log has no minutes driven |
| [Cultural preparedness](06-madurez-y-gaps.md) | 🟢 | Personal project, no team to win over |
| [Technical infrastructure](06-madurez-y-gaps.md) | 🔴 | No hardware, no pipeline |
| [Governance framework](04-riesgo-y-obligaciones.md) | 🔴 | Third-party data protection unresolved |

🟢 settled &middot; 🟡 in progress &middot; 🔴 blocking

## The pilot

```
dashcam → small model on an NVIDIA Jetson (in the car, real time)
        → clips upload over home WiFi
        → agent drafts the report
        → I review: approve or drop (human in the loop)
        → the city
```

Stage today: **envision**. Next realistic stage: **experiment** (one car, a few weeks).

## Privacy

Routes, times, plates and clips never leave my machine: they live in `privado/`, which is gitignored. This repo only shows aggregated totals. Faces and non-offending plates get masked before any report is drafted.

## Files

Written in Spanish, as studied.

| File | What it covers |
|---|---|
| [01-outcome-y-use-case.md](01-outcome-y-use-case.md) | Outcome, capability + mechanism + outcome, rules or AI, build or buy |
| [02-baseline-y-kpis.md](02-baseline-y-kpis.md) | Claim vs evidence, the three baseline checks, leading and lagging KPIs |
| [03-registro.md](03-registro.md) | Format of the private manual log |
| [04-riesgo-y-obligaciones.md](04-riesgo-y-obligaciones.md) | Risk class, human in the loop, identify → map → evidence |
| [05-bias-y-monitoreo.md](05-bias-y-monitoreo.md) | Where bias can enter, the monitoring control |
| [06-madurez-y-gaps.md](06-madurez-y-gaps.md) | Maturity stage, readiness gaps and their order |
| [decisiones.md](decisiones.md) | Every decision, dated |

## License

&copy; 2026 [Luis Barral](https://barral.dev). All rights reserved. Public to read, not to reuse. See [LICENSE](LICENSE).

AWS and AWS Certified AI Business Strategist are trademarks of Amazon.com, Inc. or its affiliates. Not affiliated with or endorsed by AWS.

<div align="center">

**[Luis Barral](https://barral.dev)** &middot; All rights reserved

<img src="assets/signature.svg" height="29" alt="co-assisted by Claude Opus 5.5">

</div>
