# tiny-chess-01-entry

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/{owner}/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/{owner}/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact chess engine in 4 KB of Python (4,038 bytes packed): 0x88 board, alpha-beta search with a transposition table, late-move reductions, quiescence search with delta pruning, and a material + piece-square evaluation. Iterative deepening under a fixed 100,000-node budget per move. Deterministic: fixed node count, no clock, no randomness. Local practice-trial Elo 1191 at 25,000 nodes (above the 1154 practice floor); ~1330–1390 extrapolated at the submitted 100,000-node budget.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:PORT python3 main.py
```

The grader runs `main.py` with `MAKEFUN_ENV_URL` set; the engine plays games over that HTTP env (POST /game, /move, /resign). Python 3.13, standard library only.

---

<sub>Entered on [make.fun](https://make.fun/?ref={referral_code}&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
