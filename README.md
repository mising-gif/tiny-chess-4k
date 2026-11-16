# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/mising-gif/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/mising-gif/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in at most 4,096 bytes of Python: a 0x88 board,
negamax search with alpha-beta and PVS, quiescence, a transposition table,
killer/history move ordering and piece-square-table evaluation with an
endgame king blend. It searches to a fixed node budget and never reads a
clock, so every game replays move for move. `main.py` is the whole engine
(the readable source, packed with the kit's `makefun compress`).

## Run it

```sh
MAKEFUN_ENV_URL=<env url> python3 main.py
```

It plays every game of the make.fun tiny-chess-01 gauntlet through the env
at that URL: `POST /game` serves the game in play, `POST /move` plays a move.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ypa0ty6s&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
