# 03 Log format

The real log lives in `private/log.md` (gitignored), because it holds routes and times.

## Row format

| Date | Time slot | Area | Minutes driven | Violation type | Count | Clip |
|---|---|---|---|---|---|---|
| 2026-11-10 | morning | Montevideo | 35 | red light | 1 | (file name) |

- **Time slot:** morning, midday, afternoon, night.
- **Area:** Montevideo or Canelones (no exact route in the public version).
- **Minutes driven:** the field that turns a count into a comparable rate.
- **Violation type:** per the written rule, not per what bothers me.
