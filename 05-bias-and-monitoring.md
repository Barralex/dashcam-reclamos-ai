# 05 Bias and monitoring

## Where bias can enter

| Stage | Risk in this case | Fix |
|---|---|---|
| Framing | "Violation" = whatever bothers me | Use the written rule |
| Data | Model trained on another country's streets | Evaluate it on Montevideo and Canelones clips |
| Evaluation | One global % hides gaps | Measure per violation type and day/night |
| Production use | As reviewer I can add bias (always the same cars) | Monitor my own decisions too |
| Bias drift | Only my routes get filmed | Know the map is tilted; don't generalize |

## Control (measure + threshold + owner)

- **Measure:** % of detections I drop on review.
- **Threshold:** over 40% in a week (to be calibrated).
- **Owner:** me.
- **What to check:** hallucination (one odd case), degradation (dirty lens, firmware change) or drift (winter, rain, new streets).
