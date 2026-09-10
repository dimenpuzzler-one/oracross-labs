# ORACROSS Labs — open datasets

Raw observations behind the open research published at
[oracross.com/en/labs](https://oracross.com/en/labs).

Every study here computes Bazi (四柱), Zi Wei Dou Shu (紫微斗數) and Western
astrology with the **same engines under identical conditions**. That is the only
reason these numbers exist: comparing the three requires implementing all three
in one place, which is rarely done.

| ID | Study | Published | Write-up |
|---|---|---|---|
| `ORX-LAB-001` | Birth-Time Uncertainty and Chart Stability Across Bazi, Zi Wei Dou Shu, and Western Astrology | 2026-09-06 | [read](https://oracross.com/en/labs/birth-time-sensitivity) |
| `ORX-LAB-002` | Calendar, Time-Zone, and Solar-Time Boundary Effects in Three Birth-Chart Systems | 2026-09-10 | [read](https://oracross.com/en/labs/time-conventions) |

## Files

```
datasets/orx-lab-001/observations.csv   one row per (birth time × offset)
datasets/orx-lab-001/summary.json       aggregated result the website reads
datasets/orx-lab-001/README.md          method, results, limits

datasets/orx-lab-002/observations.csv   one row per (birth time × convention)
datasets/orx-lab-002/summary.json       aggregated result the website reads
datasets/orx-lab-002/README.md          method, results, limits
```

## Reproducing

The computation lives in the product repository, not here. This repository is the
**published copy** of its output, so that a citation keeps working even if the
website changes. The method is documented in each study's `README.md`.

The calculation path contains no randomness, no wall-clock time and no external
calls, so the same command produces the same table.

## What these studies do not claim

They do not measure whether any system predicts anything, and they do not rank
the systems against each other. A stable computation is not a correct
interpretation. Each study states its own limits.

## License

Data is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Use it, including commercially; please attribute.

See `CITATION.cff` for the citation format.
