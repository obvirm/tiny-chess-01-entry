# tiny-chess-01

A chess engine for the `tiny-chess-01` bounty: the strongest engine I could fit in
4 KB of Python.

- 0x88 board; pieces and moves are packed into small integers.
- Alpha-beta with iterative deepening, a transposition table, killer and history
  move ordering, and a quiescence search over captures and promotions.
- Evaluation: material, piece-square tables and the bishop pair.
- Deterministic on purpose: a fixed node budget, never a clock and never randomness,
  so a replay reproduces the same moves.
- It speaks the contest env protocol directly over HTTP (`/game`, `/move`).

`main.py` is the whole engine: an LZMA payload of the source plus the competition's
own unpacker stub, produced by the kit's `makefun compress`. The readable source
travels with the entry's build transcripts.
