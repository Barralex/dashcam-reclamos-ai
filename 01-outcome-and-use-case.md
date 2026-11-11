# 01 Outcome and use case

## Outcome (no technology)

Increase the number of real, verifiable traffic violation reports accepted by the Montevideo and Canelones authorities.

- **Real:** an actual violation, not a false positive.
- **Verifiable:** the authority can check it from the evidence (clip, date, place).
- **Accepted:** the authority takes the report in. Reports sent is only a leading KPI.
- [ ] Target: X accepted reports per month (set once the baseline exists).

## Use case = capability + mechanism + outcome

- **Capability:** detect traffic violations on video.
- **Mechanism:** a model in the car spots the violation and keeps the clip, an agent drafts the report and pre-fills the SUR form, I review it, solve the captcha and send it.
- **Outcome:** valid reports accepted by the city.

## Rules or AI?

| Task | Decision | Why |
|---|---|---|
| Spot the violation on video | AI | The pattern isn't known in advance: light, angle, rain, every car is different. |
| Fill in the report form | Rules | Fixed format, always the same. |

## Build, buy or partner?

| Piece | Decision | Why |
|---|---|---|
| In-car detector | Build | Clips of Uruguayan streets are proprietary data: a possible data flywheel. |
| Report-drafting agent | Buy | Managed service (e.g. Amazon Bedrock): fast, no differentiation. |
