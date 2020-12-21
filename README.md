# Human-like NNUE Networks

This repository contains networks that I've developed with the goal to create various human-like styles.

## Usage

Download any of the nets under releases.

[Clone my fork of Cfish](https://github.com/kennyfrc/Cfish/tree/nps), which allows you to lower the nodes per second, achieving play that is commensurate with your ELO.

When compiling, make sure you use `pure=yes` and `nnue=yes`.

In that fork, I've modified `nodestime` (UCI option) to use nodes per second instead of nodes per millisecond.

These are the recommended settings based on ELO (rough estimates):
```
ELO   nodestime
1500  100
1800  10000
2000  100000
2500  2000000
```

Set the weight within `EvalFile`


## Roadmap

The first network developed is based on 600 million human games played OTB (from Caissabase) and [Rodent IV's](https://github.com/nescitus/rodent-iv) Moprhy personality (i.e. active, attacking, centralizing, and sacrifical playstyle). This is currently about 70 elo stronger than SF10.

```
Score of evil-morty-0.1 vs stockfish-10: 54 - 34 - 12 [0.600]
...      evil-morty-0.1 playing White: 29 - 12 - 9  [0.670] 50
...      evil-morty-0.1 playing Black: 25 - 22 - 3  [0.530] 50
...      White vs Black: 51 - 37 - 12  [0.570] 100
Elo difference: 70.4 +/- 65.8, LOS: 98.3 %, DrawRatio: 12.0 %
100 of 100 games finished.
```

Future considerations include developing the NNUE version of the [Maia chess project](https://github.com/CSSLab/maia-chess) (and eliminate its endgame problems). And targeted training around a particular player.

