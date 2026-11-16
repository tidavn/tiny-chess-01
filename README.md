# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/tidavn/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/tidavn/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 3,968 bytes of Python: 0x88 board, negamax alpha-beta
with null-move pruning, iterative deepening on a fixed 80,000-node
budget, transposition table, killer moves, MVV-LVA ordering, quiescence
over captures and promotions (and all evasions in check), and a
material + piece-square evaluation. No clock, no randomness: the same
position always gets the same move, so a live trial and its replay agree.
It plays its 8 games against the house gauntlet through the contest env.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:18080 python3 main.py
```

`main.py` is the whole engine, packed by the kit's `makefun compress`
from the readable source in `src/engine.py` (kept beside the entry for
the transcript check; it is not part of the submitted snapshot).

---

Entered on [make.fun](https://make.fun/?ref=k73yfdz2&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
