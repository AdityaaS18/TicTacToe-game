# Tic-Tac-Toe with Minimax Algorithm

This is a Python implementation of the classic Tic-Tac-Toe game featuring an AI opponent powered by the Minimax algorithm. The AI is designed to play optimally, making it unbeatable in a standard 3x3 grid.

## Features

- **Human vs AI**: Play against the computer with the AI using the Minimax algorithm.
- **Unbeatable AI**: The AI always chooses the optimal move, making it impossible to defeat.
- **Simple CLI Interface**: Easy-to-use command-line interface.

## How It Works

The Minimax algorithm is a recursive method used in decision-making and game theory. It assumes that the opponent will also play optimally. In Tic-Tac-Toe, the AI evaluates all possible moves and selects the one that maximizes its chances of winning or minimizing its chances of losing.

### Minimax Algorithm Overview

1. **Maximizer vs Minimizer**: 
    - The player (human) tries to maximize their score.
    - The AI tries to minimize the player's score.
    
2. **Recursion**: 
    - The algorithm explores all possible future moves, evaluating the board's state after each move.
    
3. **Scoring**:
    - A win for the AI is scored as `+1`.
    - A win for the player is scored as `-1`.
    - A draw is scored as `0`.

4. **Optimal Move**: 
    - The AI chooses the move with the highest minimax score.

## Getting Started

### Prerequisites

- Python 3.x

### Installation

1. Clone this repository

2. Run the Tic-Tac-Toe game

### How to Play

- The game will prompt you to choose your symbol (`X` or `O`).
- The board is represented as a 3x3 grid with positions numbered 1-9.
- Input the number corresponding to the position where you want to place your symbol.
- The AI will then make its move.
- The game continues until there's a winner or the board is full (draw).

### Example

```
Choose your symbol (X or O): X

 1 | 2 | 3 
-----------
 4 | 5 | 6 
-----------
 7 | 8 | 9 

Your move (1-9): 5

 X |   |   
-----------
   | O |   
-----------
   |   |   

Your move (1-9): 1

 X |   |   
-----------
   | O |   
-----------
 X |   |   

...
```

## Code Overview

- **`tictactoe.py`**: The main script containing the game logic, Minimax algorithm implementation, and user interface.

### Key Functions

- **`minimax(board, depth, is_maximizing)`**: Implements the Minimax algorithm to evaluate the board and determine the optimal move.
- **`evaluate(board)`**: Scores the board based on the current state.
- **`is_moves_left(board)`**: Checks if there are any available moves left on the board.
- **`find_best_move(board)`**: Determines the best move for the AI based on the Minimax algorithm.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request if you have any improvements or bug fixes.

---

Enjoy playing against an unbeatable AI!
