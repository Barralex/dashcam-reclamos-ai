# 01 Outcome and use case

## Outcome (no technology)

Cut the manual time to turn a month of dashcam captures into ready-to-send reports, from ~4 hours to under 30 minutes. I only decide which ones to send.

- **The pain:** once a month I sit with the SD card, watch every capture, pick the real violations, cut and convert the clips, and only then fill in the form.
- **Not the pain:** filling in the form. It's a fixed cost and stays manual (SUR has a captcha).
- **Guardrail:** saving time can't lower quality. Reports must stay **real** (an actual violation), **verifiable** (the authority can check the clip, date and place) and **accepted** by the authority.
- Target: under 30 minutes per month (from an **assumed** baseline, see `02`).

## Use case = capability + mechanism + outcome

- **Capability:** prepare captured clips: find the likely violations and leave them cut and in the right format.
- **Mechanism:** the clips from the SD go through a model that ranks the likely violations; each candidate gets cut and converted and lands in a review view with a draft of the report; I approve or drop it, then submit it by hand on SUR.
- **Outcome:** minutes, not hours, from SD card to ready-to-send reports, with the quality guardrail held.

## Rules or AI?

| Task | Decision | Why |
|---|---|---|
| Tell a real violation from a non-event | AI | The pattern isn't known in advance: light, angle, rain, every car is different. |
| Cut the clip around the moment and convert the format | Rules | Fixed steps once the moment is known. |
| Draft the report text | Rules first | Fixed form; a template may be enough. |
| Fill in and send the form | Manual | Captcha; fixed cost, out of scope. |

## Build, buy or partner?

| Piece | Decision | Why |
|---|---|---|
| Violation ranking model | Build | Clips of Uruguayan streets are proprietary data: a possible data flywheel. |
| Clip cutting and conversion | Buy / reuse | Standard tools, no differentiation. |
| Report drafting | Buy, if a template falls short | Managed service (e.g. Amazon Bedrock): fast, no differentiation. |

- [ ] Open: does the model need to run in the car in real time, or is processing the SD card at home enough? The pain is triage, not detection on the road.
