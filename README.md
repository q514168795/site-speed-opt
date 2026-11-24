# make.fun entry: site-generator-speed-01-run-20261122

[![make.fun bounty](https://img.shields.io/badge/make.fun-bounty-blue)](https://make.fun/bounty/site-generator-speed-01-run-20261122)
[![license](https://img.shields.io/badge/license-MIT-green)](LICENSE)

A faster `solve.js` for make.fun's static-site speed bounty. It keeps the house driver (`main.ts`) and exports
`run(input)` with output byte-for-byte identical to the reference `makefun-site 1.0.0`, on the official dev kit's
practice cases and on differential fuzzing against the reference.

Verified locally: g-0001 1,503,275 B, g-0002 2,830,687 B, g-0003 3,112,472 B — all identical.
