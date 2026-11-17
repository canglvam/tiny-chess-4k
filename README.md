# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/canglvam/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/canglvam/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python for tiny-chess-01 (MIT).

`main.py` is the whole engine: 0x88 board, alpha-beta with a
transposition table, killers, history and MVV-LVA ordering, quiescence
search, check extensions and pin-based legality, and iterative
deepening to a fixed node budget per move, so it is deterministic.
It plays through the env at `MAKEFUN_ENV_URL`.
`engine.py` (not committed) is the readable source `main.py` was
packed from with `makefun compress`.
