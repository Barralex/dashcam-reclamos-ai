# 01 Outcome and use case

## Outcome (no technology)

The city receives reports of real traffic violations, with evidence it can act on.

- [ ] Target: X valid reports per month (set once the baseline exists).

## Use case = capability + mechanism + outcome

- **Capability:** detect traffic violations on video.
- **Mechanism:** a model in the car spots the violation and keeps the clip, an agent drafts the report, a person reviews it and sends it.
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
