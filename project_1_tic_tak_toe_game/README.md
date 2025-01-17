# Tic Tak Toe

This is a simple game of tic tac toe written in Python. The game is played between two players, who take turns marking the spaces in a 3x3 grid. The player who succeeds in placing three of their marks in a horizontal, vertical, or diagonal row is the winner.

## Glossary

- [Tic Tak Toe](#tic-tak-toe)
  - [Glossary](#glossary)
  - [Game Layout](#game-layout)
  - [Gameplay](#gameplay)
  - [Functions](#functions)
    - [game\_board](#game_board)
    - [user\_pic](#user_pic)
    - [user\_choice](#user_choice)
    - [continue\_game](#continue_game)
    - [board\_replace](#board_replace)
    - [check\_win](#check_win)
    - [choose\_first](#choose_first)
    - [reset\_board](#reset_board)
    - [board\_full\_check](#board_full_check)
    - [proceed](#proceed)
    - [game\_over](#game_over)
    - [log\_score](#log_score)
    - [set\_names](#set_names)
    - [board\_update](#board_update)
  - [Project Structure](#project-structure)
  - [Installation](#installation)
  - [Libraries](#libraries)

## Game Layout

The game board is made up of nine squares, each identified by a number ranging from 1 to 9. The board is set up as follows:

| 7   | 8   | 9   |
| --- | --- | --- |
| 4   | 5   | 6   |
| 1   | 2   | 3   |

## Gameplay

The game begins with Player 1 selecting which side they will play (X or O). Player 1 will then pick a position on the board they wish to place their mark by entering the corresponding number. This will be followed by Player 2 doing the same. The game will continue until either one of the players has successfully placed three of their marks in a row, or until all of the spots on the board are taken, in which case the game is a tie.

## Functions

The game uses several functions to run.

### game_board

This function is used to draw the game board.

### user_pic

This function is used to have the players select which side they wish to play. The function will prompt the player to enter either an X or O.

### user_choice

This function is used to have the players pick a position on the board. The function will prompt the player to enter a number from 1 to 9.

### continue_game

This function is used to ask the players if they wish to continue playing. The function will prompt the player to enter either Yes or No.

### board_replace

This function is used to replace the board with the player's mark.

### check_win

This function is used to check if either player has won the game.

### choose_first

Randomly selects a player to go first

### reset_board

Sets all the values to default

### board_full_check

Checks if the board is full or not

### proceed

Asks the user if they want to start the game

### game_over

Shows overall game score (game over screen)

### log_score

Writes down overall game score after players done playing into _'scores.txt'_.
Structure of a log file is: 'date, name, score'

### set_names

Asks players to enter their names to be used in the output and _'scores.txt'_.

### board_update

Updates a game board according to changes in the game_lisе

## Project Structure

Project contains 4 files:

- [tic_tak_toe.ipynb](./tic_tak_toe.ipynb) - Jupiter notebook with development stages and steps.
- [tic_tak_toe.py](./tic_tak_toe.py) - a python script, containing main code of the project.
- [requirements.txt](./requirements.txt) - a list of python modules and versions.
- [README.md](./README.md) - this file.

## Installation

```Git
git clone --no-checkout https://github.com/shohart/ shohart
cd shohart
git sparse-checkout init --cone
git sparse-checkout set UDEMY-python-projects/project_1_tic_tak_toe_game
```

## Libraries

- random
- datetime
- os
- art
