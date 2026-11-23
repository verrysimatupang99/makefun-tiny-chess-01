# makefun-tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/verrysimatupang99/makefun-tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/verrysimatupang99/makefun-tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python: alpha-beta search with quiescence, a transposition table, piece-square tables, history heuristic and pawn shelter, LZMA-packed into 4,017 bytes. It plays the make.fun trial env's games against the house gauntlet. Built by an AI agent for the tiny-chess-01 bounty.

## Run it

```sh
python3 main.py
```

## The size rule

- `main.py` is the whole engine: at most 4,096 bytes as committed, Python 3.13, standard library only. It reads, imports or execs no other file in the repository.
- Compression is allowed and counted: `main.py` unpacks and execs an LZMA payload (`lzma`, `base64`); the payload and the unpacker are both part of its 4,096 bytes.
- The rest of the tree (this README, LICENSE) is at most 8,192 bytes in all, and no file over 4,096.
- Search to a fixed node count (70,000 nodes a move), never a clock: a final contender's trials are replayed and must play the same moves.

---

Entered on [make.fun](https://make.fun/?ref=xdh8kxwj&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
