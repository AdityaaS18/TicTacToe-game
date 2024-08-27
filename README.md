# Tic-Tac-Toe Game with Minimax Algorithm

This is a Python implementation of the classic Tic-Tac-Toe game, where you can play against another player or an AI opponent that uses the Minimax algorithm for making optimal moves.

## Features

- **Single Player Mode**: Play against the computer (AI).
- **Multiplayer Mode**: Play against another human player.
- **Command-Line Interface**: Simple, text-based interface.

## How It Works

### Game Modes

1. **Single Player Mode**: 
    - You play as `X`, and the computer plays as `O`.
    - The AI uses the Minimax algorithm, making it extremely challenging to beat.
    
2. **Multiplayer Mode**:
    - Two players can take turns playing as `X` and `O`.
    - No AI involvement in this mode; both players are human.

### Minimax Algorithm

The Minimax algorithm is implemented to allow the computer to make the best possible move by simulating all possible game states. The AI evaluates each possible move and selects the one that maximizes its chances of winning or minimizing its chances of losing.

### Board Representation

The Tic-Tac-Toe board is represented as a list of 9 positions:

- `0` - Empty spot
- `-1` - Player `X`
- `1` - Player `O` or the AI

## Getting Started

### Prerequisites

- Python 3.x

### Running the Game

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/tictactoe-minimax.git
   cd tictactoe-minimax
   ```

2. Run the game:

   ```bash
   python tictactoe.py
   ```

### How to Play

1. **Choose Game Mode**:
   - Enter `1` for Single Player mode (you vs. AI).
   - Enter `2` for Multiplayer mode (you vs. another player).
   
2. **In Single Player Mode**:
   - Select whether to play first (`1`) or second (`2`).
   - Input the position (1-9) where you want to place your `X`.

3. **In Multiplayer Mode**:
   - Player `X` goes first.
   - Both players will take turns inputting their desired positions.

### Board Layout

```
 1 | 2 | 3 
-----------
 4 | 5 | 6 
-----------
 7 | 8 | 9 
```

Input the number corresponding to the position where you want to place your symbol.

### Example Game Play

```
Enter 1 for Single Player, 2 for Multiplayer: 1
Computer: O vs. You: X
Enter to play 1(st) or 2(nd): 1
Current State of the Board:

_ _ _ 
_ _ _ 
_ _ _ 

Enter X's position from [1,2,3,....,9]: 5
```

The game continues until there's a winner or the board is full.

## Code Overview

- **`ConstBoard(board)`**: Displays the current state of the board.
- **`User1Turn(board)`**: Handles Player X's move.
- **`User2Turn(board)`**: Handles Player O's move in Multiplayer mode.
- **`minmax(board, player)`**: Implements the Minimax algorithm to determine the optimal move for the AI.
- **`CompTurn(board)`**: Executes the AI's move using Minimax.
- **`analyzeboard(board)`**: Analyzes the board to check for a winner or a draw.
- **`main()`**: The main function to start the game, allowing selection between single-player and multiplayer modes.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to discuss any changes or improvements.

---

Enjoy playing Tic-Tac-Toe against an unbeatable AI or challenge your friends in multiplayer mode!
