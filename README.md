# tiny-chess-01

A chess engine in at most 4,096 bytes of Python (3.13, stdlib only).

- `main.py` — the engine (4,093 bytes). Deterministic alpha-beta search
  with transposition table, killer moves, MVV-LVA ordering and quiescence,
  fixed 8,000-node budget per move. Speaks the make.fun env protocol
  (`POST /game`, `POST /move` with UCI).
- Practice Elo ~1,396 (mean over 3 trials), above the 1,154 final gate and
  above the sunfish 4 KB baseline (1,365).

Entry for make.fun bounty "Build the strongest chess engine in 4 KB of
Python" (tiny-chess-01). MIT licensed.
