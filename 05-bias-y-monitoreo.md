# 05 Bias y monitoreo

## Por dónde puede entrar el bias

| Etapa | Riesgo en este caso | Fix |
|---|---|---|
| Framing | "Infracción" = lo que me molesta | Usar la norma escrita |
| Data | Modelo entrenado con calles de otro país | Evaluarlo con clips de Montevideo y Canelones |
| Evaluation | Un % global esconde diferencias | Medir por tipo de infracción y día/noche |
| Production use | Como revisor puedo sesgar (siempre los mismos autos) | Monitorear también mis decisiones |
| Bias drift | Solo se filma por donde manejo | Saber que el mapa queda inclinado; no generalizar |

## Control (medida + threshold + owner)

- **Medida:** % de detecciones que descarto al revisar.
- **Threshold:** más de 40% en una semana (a calibrar).
- **Owner:** yo.
- **Qué revisar:** hallucination (un caso raro), degradation (cámara sucia, cambio de firmware) o drift (invierno, lluvia, calles nuevas).
