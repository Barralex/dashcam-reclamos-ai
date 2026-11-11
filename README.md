<div align="center">

# Dashcam street reports, by the book

[![Framework](assets/badges/framework.svg)](#the-brief)
[![Stage](assets/badges/stage.svg)](#the-board)
[![Blocking gaps](assets/badges/blocking.svg)](#the-board)
[![Raw data](assets/badges/privacy.svg)](#privacy)
[![License](assets/badges/license.svg)](LICENSE)

### An AI idea taken through the AIB-C01 framework before a single line of code.

A month of dashcam captures, triaged into ready-to-send reports in minutes instead of hours.<br>
A person still decides and sends every one. This repo is the business case, not the build.

</div>

---

## The brief

I report traffic violations by hand. Every day I press the dashcam button; once a month I sit with the SD card for about four hours, watch every capture, pick the real ones, cut and convert the clips, and only then file them. The form isn't the problem; the triage is. The idea is to let a model rank the likely violations and leave the clips ready, so I only decide which ones to send.

Instead of starting with the hardware, this repo runs the idea through what the [AWS Certified AI Business Strategist](https://github.com/Barralex/aws-ai-business-strategist) exam teaches: outcome first, rules or AI, build or buy, a credible baseline, risk and obligations, bias, monitoring, maturity and readiness gaps. Each question I can't answer yet becomes an open gap on the board.

**Outcome:** cut the manual time to turn a month of dashcam captures into ready-to-send reports, from ~4 hours to under 30 minutes, without lowering report quality (real, verifiable, accepted).

## The board

The weakest dimension decides, not the average.

| Piece | Status | Open gap |
|---|---|---|
| [Outcome and use case](01-outcome-and-use-case.md) | 🟡 | Outcome pivoted to triage time; in the car vs at home is open |
| [Baseline and KPIs](02-baseline-and-kpis.md) | 🔴 | Triage baseline is mock data; needs one real SD session |
| [Risk and obligations](04-risk-and-obligations.md) | 🔴 | Montevideo: does SUR take traffic violations? Canelones: no channel found |
| [Bias and monitoring](05-bias-and-monitoring.md) | 🟡 | No per-group measure defined |
| [Leadership alignment](06-maturity-and-gaps.md) | 🟢 | Roles split: Claude is executive sponsor and strategist, I am owner, builder and human in the loop |
| [Data quality](06-maturity-and-gaps.md) | 🔴 | Manual log has no minutes driven |
| [Cultural preparedness](06-maturity-and-gaps.md) | 🟢 | Personal project, no team to win over |
| [Technical infrastructure](06-maturity-and-gaps.md) | 🔴 | No hardware, no pipeline |
| [Governance framework](04-risk-and-obligations.md) | 🔴 | Third-party data protection unresolved |

🟢 settled &middot; 🟡 in progress &middot; 🔴 blocking

## The pilot

```
dashcam (button + automatic events) → SD card
        → model ranks the likely violations (in the car or at home: open)
        → clips cut and converted, report drafted, in a review view
        → I review: approve or drop (human in the loop)
        → I submit it by hand on SUR (captcha)
        → the city
```

Stage today: **envision**. Next realistic stage: **experiment** (one car, a few weeks).

## Privacy

Routes, times, plates and clips never leave my machine: they live in `private/`, which is gitignored. This repo only shows aggregated totals. Faces and non-offending plates get masked before any report is drafted.

## Files

| File | What it covers |
|---|---|
| [01-outcome-and-use-case.md](01-outcome-and-use-case.md) | Outcome, capability + mechanism + outcome, rules or AI, build or buy |
| [02-baseline-and-kpis.md](02-baseline-and-kpis.md) | Claim vs evidence, the three baseline checks, leading and lagging KPIs |
| [03-log-format.md](03-log-format.md) | Format of the private manual log |
| [04-risk-and-obligations.md](04-risk-and-obligations.md) | Risk class, human in the loop, identify → map → evidence |
| [05-bias-and-monitoring.md](05-bias-and-monitoring.md) | Where bias can enter, the monitoring control |
| [06-maturity-and-gaps.md](06-maturity-and-gaps.md) | Maturity stage, readiness gaps and their order |
| [decisions.md](decisions.md) | Every decision, dated |
| [CLAUDE.md](CLAUDE.md) | How the AI Business Strategist works: role, method, privacy and repo rules |

## License

&copy; 2026 [Luis Barral](https://barral.dev). All rights reserved. Public to read, not to reuse. See [LICENSE](LICENSE).

AWS and AWS Certified AI Business Strategist are trademarks of Amazon.com, Inc. or its affiliates. Not affiliated with or endorsed by AWS.

<div align="center">

**[Luis Barral](https://barral.dev)** &middot; All rights reserved

<img src="assets/signature.svg" height="29" alt="co-assisted by Claude Opus 5.5">

</div>
