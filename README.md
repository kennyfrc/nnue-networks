# Human-like NNUE Networks

This repository contains networks that I've developed with the goal to create various human-like styles. 

This is inspired by the Maia chess project and I wanted to make versions for [Stockfish NNUE](https://github.com/CSSLab/maia-chess). The con of the Maia bots is that it had endgame and tactical problems. Most engines are either too strong tactically or positionally. This aims to provide a more authentic sparring experience for players.

## Play At Lichess

You can play against these bots at Lichess through these links:
* [nnuehuman1200](https://lichess.org/@/nnuehuman1200)
* [nnuehuman1500](https://lichess.org/@/nnuehuman1500)
* [nnuehuman2400](https://lichess.org/@/nnuehuman2400)

## Play on your computer

If you want a local version on your computer, fork my [cfish repository](https://github.com/kennyfrc/Cfish) and follow the instructions there. I've made 3 branches named `elo1200`, `elo1600`, and `elo2300`. I know the elos there and at lichess are inconsistent. Fill fix those on a later date.

## Just the nets

See [releases](https://github.com/kennyfrc/nnue-networks/releases).


## Fixed NPS testing results

An interesting observation from my fixed NPS testing is that if you pool together 1200, 1500, and 2400 in a 50k nps tournament (used `tc=40/60`), the estimated elos perfectly arrange themselves into 1200, 1500, and 2400. 

```
Rank  Name  Elo +/- Games Wins  Losses  Draws Points  Score Draw

1 cfish-kb2300  657 176 180 173 1 6 176.0 97.8% 3.3%

2 shredder-1500 -54 50  180 71  99  10  76.0  42.2% 5.6%

3 cfish-l1600 -62 50  180 69  101 10  74.0  41.1% 5.6%

4 cfish-l1200 -253  63  180 29  141 10  34.0  18.9% 5.6%


360 of  360 games finished.
```