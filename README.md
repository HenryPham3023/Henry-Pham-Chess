# Henry Pham's SupremeChess Engine

## Table of contents
* [General info](#general-info)
* [Engine Improvements TODO](#engine-improvements-todo)
* [UI TODO](#ui-todo)
* [Instructions](#instructions)
* [Further development ideas](#further-development-ideas)


[Eddie's YouTube channel](https://www.youtube.com/channel/UCaEohRz5bPHywGBwmR18Qww)

[First episode of "Chess engine in Python"](https://www.youtube.com/playlist?list=PLBwF487qi8MGU81nDGaeNE1EnNEPYWKY_)

# Henry's Chess

Henry Chess is a Python/Pygame desktop chess application created for the Year 12 Software Engineering Major Project. It includes local chess, rated AI bots, puzzles, premoves, Stockfish game review, themes, time controls, and executable support.

## Features

* Local two-player chess
* Rated AI bots
* Practice bot mode
* Puzzle training
* Stockfish-powered game review
* Move labels, accuracy and best-move feedback
* Premove support
* Graphical arrows and square highlights
* Board and piece themes
* Time controls
* PGN/FEN import
* Executable build support

## How to Run from Source

1. Download or clone the project.
2. Open the project folder in VS Code.
3. Install requirements:

```bash
python -m pip install -r requirements.txt
```

4. Run the game:

```bash
python ChessMain.py
```

On Mac, use:

```bash
python3 ChessMain.py
```

## Running the Executable

1. Download the ZIP file.
2. Extract the ZIP file.
3. Open the extracted `Henry Chess` folder.
4. Double-click `Henry Chess.exe`.

Do not remove the `.exe` from its folder, because the app needs the included assets, sounds, images and Stockfish files to run properly.

Do not remove the files from the extracted folder, because the game needs its assets, sounds, pieces and Stockfish files.

## Stockfish Setup

Stockfish is optional but recommended for stronger Game Review and higher-rated bots.

Windows path:

```text
engines/stockfish/windows/stockfish.exe
```

Mac path:

```text
engines/stockfish/mac/stockfish
```

The file name must be exactly `stockfish.exe` on Windows or `stockfish` on Mac.

## Controls

| Action           | Control                |
| ---------------- | ---------------------- |
| Select piece     | Left click             |
| Move piece       | Left click destination |
| Draw arrow       | Right click drag       |
| Highlight square | Right click            |
| Premove          | Use the Premove button |
| Change theme     | Board / Pieces buttons |
| Review game      | Game Review button     |

## Project Structure

```text
ChessMain.py          Main app and interface
ChessEngine.py       Chess rules and legal moves
SmartMoveFinder.py   AI and bot logic
stockfish_review.py  Stockfish game review
game_io.py           PGN/FEN and file handling
assets/              Images and sounds
engines/             Stockfish files
docs/                Documentation
tests/               Unit tests
```

## Testing

Run:

```bash
pytest -q
```

## Acknowledgements

This project uses Python, Pygame and optional Stockfish integration. Stockfish is third-party open-source software used for game analysis and stronger bot play.

## Developer

Created by Henry for the Year 12 Software Engineering Major Project.

GitHub Repository:

```text
https://github.com/HenryPham3023/Henry-Pham-Chess
```
