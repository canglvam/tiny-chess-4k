# tiny-chess

A chess engine in 4 KB of Python for tiny-chess-01 (MIT).

`main.py` is the whole engine: 0x88 board, alpha-beta with a
transposition table, killers, history and MVV-LVA ordering, quiescence
search, check extensions and pin-based legality, and iterative
deepening to a fixed node budget per move, so it is deterministic.
It plays through the env at `MAKEFUN_ENV_URL`.
`engine.py` (not committed) is the readable source `main.py` was
packed from with `makefun compress`.
