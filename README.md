# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/banishwor/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/banishwor/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python: negamax search with alpha-beta pruning, a transposition table, quiescence search, null-move pruning and a tapered piece-square evaluation. It plays the make.fun tiny-chess gauntlet through the contest env on a deterministic per-game node budget — never a clock, so every game replays move for move.

## Local practice results

Graded with the kit's own practice trials (6 games each against the house gauntlet):

- Trial 0: Elo 1,455 — wins vs depth-2, nodes-100k and nodes-250k, draw vs depth-3
- Trial 1: Elo 1,545
- Trial 2: Elo 1,654

The practice floor for the final is 1,154; the house baseline (sunfish's 4 KB NNUE entry) averages about 1,365 on the same sets.

## Run it

```sh
MAKEFUN_ENV_URL=http://store:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=REFCODE&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
