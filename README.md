# Tic-tac-toe_solver
This is a code for a game called Tic-Tac-Toe solver
# Tic-Tac-Toe Game with AI

This is a Python implementation of the classic Tic-Tac-Toe game, where a player can challenge either their own strategic thinking or an AI opponent. The game offers two difficulty levels for the AI: **easy** (random moves) and **hard** (optimal moves using the Minimax algorithm).

## Features

- **Two Difficulty Levels**:
  - **Easy**: AI makes random moves.
  - **Hard**: AI makes optimal moves using the Minimax algorithm.
  
- **Game Flow**:
  - Players alternate turns.
  - The game ends when a player wins, or the board is full (draw).
  
- **Input**: The player selects a move by entering a number between 1 and 9, corresponding to an empty cell on the board.
  
- **Winning Condition**: A player wins by getting three of their symbols (either "X" or "O") in a row, column, or diagonal.

## How to Play

1. **Start the Game**: The game begins with a 3x3 grid, all cells empty.
2. **Choose Difficulty**: The player will be prompted to choose the difficulty level for the AI:
   - **easy**: AI makes random moves.
   - **hard**: AI uses the Minimax algorithm to make optimal moves.
3. **Player’s Move**: Enter a number between 1 and 9 to place your symbol (O) in the corresponding position on the grid.
4. **AI’s Move**: After your move, the AI will make its move.
5. **Game Continuation**: The game will continue until there is a winner or a draw.
6. **End Condition**:
   - The game ends when a player wins or when all cells are filled (draw).

## Example of Gameplay

```
Welcome to Tic-Tac-Toe!
Choose AI Difficulty (easy / hard): hard

Player's Move:
1 | 2 | 3
---------
4 | 5 | 6
---------
7 | 8 | 9

Enter your move (1-9): 5

Your Move:
X | O | X
---------
O | X | O
---------
X | O | X

Congratulations, you win!
```

## How the AI Works

The AI behavior is determined by the selected difficulty level:

### **Easy Difficulty**:
- The AI randomly selects an empty cell and places its symbol (`X`).
- This algorithm doesn't involve any strategic thinking, making it suitable for casual players.

### **Hard Difficulty**:
- The AI uses the **Minimax algorithm** to evaluate all possible future moves and select the best one.
- The AI always plays optimally and will never make an incorrect move, making it a challenging opponent.

### **Minimax Algorithm**:
- The Minimax algorithm simulates all potential game states and assigns scores based on the outcomes (win, loss, or draw).
- The AI maximizes its score (win) and minimizes the player's score (loss), choosing the move that guarantees the best possible outcome.

## Installation and Usage

To play the game, follow these steps:

1. **Clone or Download** the repository to your local machine.

2. **Install Python** (if not already installed). The game is implemented in Python 3.x.

3. **Run the Game**:
   - Navigate to the directory containing the Tic-Tac-Toe script.
   - Open a terminal or command prompt and execute the script by running:
     ```bash
     python tic_tac_toe.py
     ```

4. Follow the on-screen prompts to play the game.

## Code Structure

### Main Functions:
- **`print_board(board)`**: Prints the current state of the game board.
- **`check_winner(board)`**: Checks if a player has won the game.
- **`is_draw(board)`**: Checks if the game has ended in a draw.
- **`minimax(board, is_maximizing)`**: Recursively evaluates all possible future game states using the Minimax algorithm (for hard difficulty).
- **`find_best_move(board, difficulty)`**: Finds the best move for the AI based on the selected difficulty.
- **`user_move(board)`**: Handles player input and updates the game board with the player's move.
- **`play_game()`**: The main game loop that drives the gameplay, alternating between the player's and AI's turns.

## Requirements

- **Python 3.x**: The game is written in Python and requires Python 3.x to run.

## License

This project is open-source and can be freely used, modified, and distributed under the MIT License.

---

Enjoy the game, and may the best player win!
