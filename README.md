# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/bg4sgp/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/bg4sgp/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4 KB of Python (main.py is the whole engine, shipped as an lzma payload with its unpacker). It plays the make.fun tiny-chess-01 gauntlet through the env API: negamax alpha-beta search with iterative deepening under a fixed node budget (fully deterministic, no clock), principal-variation search, a transposition table with mate-score adjustment, in-search repetition detection, and a quiescence search over captures and promotions that resolves all check evasions when in check, over a 0x88 board with a piece list and incremental Zobrist hashing. Evaluation is material plus tapered piece-square tables (middlegame/endgame king tables blended by phase).

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=ww39pck3&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
