# Tic-Tac-Toe Game

This repository contains a C++ implementation of the classic Tic-Tac-Toe game. The game allows a human player to compete against an AI computer player that uses the minimax algorithm to make optimal moves.

## Features

- **Player Symbols**: Human player uses 'X' and the computer uses 'O'.
- **Interactive Board Display**: The current state of the board is displayed after each move.
- **User Instructions**: Provides clear instructions on how to play and the mapping of cell numbers to board positions.
- **AI Logic**: The computer player is implemented using the minimax algorithm, ensuring optimal moves.
- **Win and Draw Detection**: Checks for winning conditions and detects draws.
- **User Choice**: Players can choose whether to start first or let the computer start.

## How to Play

1. **Starting the Game**: The game prompts the player to choose whether they want to start first. Enter 'y' to start first or 'n' to let the computer start.
2. **Making Moves**: Players take turns entering the cell number (1-9) where they want to place their symbol.
3. **Win or Draw**: The game will announce the winner once a winning condition is met or declare a draw if the board is full with no winner.
4. **Play Again**: After the game ends, the player can choose to play another game or quit.

## How to Compile and Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/tic-tac-toe.git
    cd tic-tac-toe
    ```

2. **Compile the Program**:
    ```bash
    g++ -o tictactoe tictactoe.cpp
    ```

3. **Run the Program**:
    ```bash
    ./tictactoe
    ```

## Code Overview

### Main Functions

- **showBoard**: Displays the current state of the board.
- **showInstructions**: Provides instructions on how to play and the cell numbering.
- **initialise**: Initializes the game board by setting all positions to '*'.
- **declareWinner**: Announces the winner of the game.
- **rowCrossed, columnCrossed, diagonalCrossed**: Check if any row, column, or diagonal has the same symbol, indicating a win.
- **gameOver**: Checks if the game has ended either due to a win or a draw.
- **minimax**: AI algorithm to determine the best move for the computer by simulating all possible moves and their outcomes.
- **bestMove**: Determines the optimal move for the computer based on the current board state using the minimax function.
- **playTicTacToe**: Main game function that handles the gameplay loop, alternating turns between the human and the computer, and managing user input and game state.
- **main**: Entry point of the program, handles the initial user input for starting the game and the choice of who goes first, and manages the game replay loop.
