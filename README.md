# Human-like NNUE Networks

This repository contains networks that I've developed with the goal to create various human-like styles. 

This is inspired by the Maia chess project and I wanted to make versions for [Stockfish NNUE](https://github.com/CSSLab/maia-chess). The con of the Maia bots is that it had endgame and tactical problems. Most engines are either too strong tactically or positionally. This aims to provide a more authentic sparring experience for players.

## Download the Nets

See [releases](https://github.com/kennyfrc/nnue-networks/releases).

For now, I only recommend the "Distilled Maia" nets. These are generated from self-play Maia 1900 games (30m positions).

## Scripts

To see the scripts I used to generate these nets, see "scripts". These uses this [specific commit](https://github.com/nodchip/Stockfish/commit/36092b855a5e2bcfb587a36e2055ea068e4bd8e5) of the nodchip library.