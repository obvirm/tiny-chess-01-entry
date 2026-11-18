# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/obvirm/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/obvirm/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine for the make.fun bounty: 0x88 board, alpha-beta search with
iterative deepening, transposition table, MVV-LVA ordered moves and a quiescence
search. The engine uses a fixed node budget instead of a clock, so it is
deterministic across live and replay trials.

`main.py` is the whole engine, packed with the competition's own `makefun compress`.
The readable source travels with the entry's build transcripts.

Run: `python3 -P -s main.py` with `MAKEFUN_ENV_URL` provided by the contest env.
