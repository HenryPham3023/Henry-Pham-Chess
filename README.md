# Python Chess Engine

## Table of contents
* [General info](#general-info)
* [Engine Improvements TODO](#engine-improvements-todo)
* [UI TODO](#ui-todo)
* [Instructions](#instructions)
* [Further development ideas](#further-development-ideas)


[Eddie's YouTube channel](https://www.youtube.com/channel/UCaEohRz5bPHywGBwmR18Qww)

[First episode of "Chess engine in Python"](https://www.youtube.com/playlist?list=PLBwF487qi8MGU81nDGaeNE1EnNEPYWKY_)

## Instructions
1. Clone this repository 
2. Run `python3 -m pip install -r ./requirements.txt`
3. Run `python3 ChessMain.py`.
4. Enjoy the game!

![PvP Chess Game with move logger](./assets/baord01.png)

#### Keys:
* Press `z` to undo a move.
* Press `r` to reset the game.

#### Notes: 
* For now, the game runs with PvP mode enabled.

## Further development ideas
1. Move ordering - look at checks, captures and threats first, prioritize castling/king safety, look at pawn moves last (this will improve alpha-beta pruning). Also start with moves that previously scored higher (will also improve pruning).
2. Hash board positions already visited to improve computation time for transpositions, so that after a move is made the engine doesn't have to recalculate all the moves.
3. Evaluating kings placement on the board (separate in middle game and in the late game).
4. Book of openings.
