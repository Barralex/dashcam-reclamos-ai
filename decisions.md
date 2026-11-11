# Decisions

- 2026-11-10: routes, times, plates and clips are not published. They live in `private/` (gitignored); the repo only shows totals.
- 2026-11-10: the log measures violations per hour driven, not just a count, because time in each area isn't comparable.
- 2026-11-10: the whole repo is written in English.
- 2026-11-10: Claude acts as the AI Business Strategist on this project: it leads the process and recommends, Luis decides. No re-teaching the course.
- 2026-11-10: outcome set: increase the number of real, verifiable reports sent to the Montevideo and Canelones authorities.
- 2026-11-11: the outcome stays channel-agnostic; any official channel that accepts the evidence counts.
- 2026-11-11: the pilot starts with Montevideo only. Canelones stays an open gap until it has a reporting channel.
- 2026-11-11: outcome changed from reports sent to reports accepted by the authorities. Reports sent becomes a leading KPI.
- 2026-11-11: on SUR the agent only drafts and pre-fills the report. Luis solves the captcha and submits. No automated submission, no captcha bypass.
- 2026-11-11: mechanism corrected: the captcha comes first, so the agent can't pre-fill SUR. It leaves a "ready to send" package in a folder and Luis submits by hand.
- 2026-11-11: outcome pivot: the pain is the monthly SD triage, not the form. New outcome: cut manual triage from ~4 h to under 30 min per month. Real, verifiable and accepted reports become the quality guardrail.
- 2026-11-11: capability changes to preparing captured clips (rank likely violations, cut, convert). Whether the model must run in the car is now open.
- 2026-11-11: the triage baseline uses mock numbers for practice; it must be replaced with one real SD session before the gate to experiment.
- 2026-11-11: roles split for practice: Claude is executive sponsor (approves each gate) and AI Business Strategist; Luis is owner, builder and human in the loop.
