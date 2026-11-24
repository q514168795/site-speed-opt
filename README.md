# make.fun entry: site-generator-speed-01-run-20261122

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/q514168795/site-speed-opt/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/q514168795/site-speed-opt/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster `solve.js` for [make.fun](https://make.fun)'s static-site speed bounty,
[site-generator-speed-01-run-20261122](https://make.fun/bounty/site-generator-speed-01-run-20261122).

It keeps the house driver (`main.ts`) and exports `run(input)` with output byte-for-byte identical to the
reference `makefun-site 1.0.0`, on the official dev kit's practice cases and under differential fuzzing.

```
node main.ts      # reads $MAKEFUN_INPUT_DIR/cases.json, writes $MAKEFUN_OUTPUT_DIR/answers.json
```

Verified locally: g-0001 1,503,275 B, g-0002 2,830,687 B, g-0003 3,112,472 B — all identical; wall time
0.26 s / 0.36 s / 0.43 s for the reference against 0.17 s / 0.24 s / 0.25 s for this entry.
