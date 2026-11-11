# 01 Outcome y use case

## Outcome (sin tecnología)

La intendencia recibe denuncias de infracciones reales, con evidencia que puede usar.

- [ ] Número objetivo: X denuncias válidas por mes (a definir con el baseline).

## Use case = capability + mechanism + outcome

- **Capability:** detectar infracciones de tránsito en video.
- **Mechanism:** un modelo en el auto detecta y guarda el clip, un agente arma la denuncia, una persona revisa y envía.
- **Outcome:** denuncias válidas aceptadas por la intendencia.

## ¿Reglas o AI?

| Tarea | Decisión | Por qué |
|---|---|---|
| Detectar la infracción en video | AI | El patrón no se conoce de antemano: luz, ángulo, lluvia, cada auto distinto. |
| Armar el formulario de la denuncia | Reglas | Formato fijo, siempre igual. |

## ¿Build, buy o partner?

| Pieza | Decisión | Por qué |
|---|---|---|
| Detector en el auto | Build | Los clips de calles uruguayas son datos propios: posible data flywheel. |
| Agente que arma la denuncia | Buy | Servicio managed (ej. Amazon Bedrock): rápido y sin diferenciación. |
