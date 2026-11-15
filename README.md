# token-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/ryan-akmal/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/ryan-akmal/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token launch radar: 289 pre-token protocols ranked by comps-calibrated implied value, with a farm plan for each. The model prices every protocol off the median FDV/TVL of live-token protocols in its own category (from the same sealed DefiLlama snapshot), then adjusts for size, seven-day growth, age with no token, and chain breadth. The dashboard is a static page — board, detail view for every protocol, filters, top-10 chart, and the comparables table — that renders with no network.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input path/to/snapshot.json
```

`main.ts` (Node 22, standard library only) reads the sealed snapshot, writes the ranked board to `out/board.json`, the dashboard data to `out/data.js`, and copies `dashboard/` and `screenshots/` to `out/`, then writes `out/dossier.json` with the vendored make.fun library.

---

<sub>Entered on [make.fun](https://make.fun/?ref=tf75e7z1&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
