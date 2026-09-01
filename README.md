# 🎮 Tic Tac Toe AI — Minimax Algorithm

A simple **Tic Tac Toe game built with Python and Tkinter**, featuring an unbeatable computer opponent powered by the **Minimax algorithm**.

The player plays as **X**, while the computer plays as **O**. The AI evaluates possible future moves and chooses the move that provides the best possible outcome.

---

## 📌 Features

* 🎮 Interactive 3×3 Tic Tac Toe board
* 🤖 AI opponent powered by the Minimax algorithm
* 🧠 AI evaluates possible game states before making a move
* 👤 Player uses **X**
* 💻 Computer uses **O**
* 🏆 Automatic winner detection
* 🤝 Automatic draw detection
* 🔄 Restart Game button
* 🖥️ Simple graphical interface using Tkinter
* ⏱️ Small delay before the AI makes its move for a more natural gameplay experience

---

## 🧠 How the AI Works

The computer uses the **Minimax algorithm**, a decision-making algorithm commonly used in two-player games.

The algorithm explores the possible moves from the current game state and assigns scores to the outcomes:

| Game Result   | Score |
| ------------- | ----: |
| Computer wins |  `+1` |
| Player wins   |  `-1` |
| Draw          |   `0` |

The AI attempts to **maximize its score**, while assuming that the player will make moves that **minimize the AI's score**.

This allows the computer to select the strongest available move.

### Minimax Process

```text
Current Board
      ↓
Check possible AI moves
      ↓
Simulate each move
      ↓
Simulate player's responses
      ↓
Continue until game ends
      ↓
Evaluate each outcome
      ↓
Choose the best move
```

Because Tic Tac Toe has a relatively small game state, the program can evaluate the possible moves directly without requiring a machine-learning model.

---

## 🛠️ Technologies Used

* **Python 3**
* **Tkinter** — Graphical User Interface
* **Math module** — Used for positive and negative infinity
* **Minimax Algorithm** — AI decision making

No external Python packages are required.

---

## 📂 Project Structure

```text
Tic-Tac-Toe-AI/
│
├── tic_tac_toe.py
└── README.md
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Mrmanticore/Tic-Tac-Toe-AI.git
```

### 2. Open the project directory

```bash
cd Tic-Tac-Toe-AI
```

### 3. Run the game

```bash
python tic_tac_toe.py
```

> **Note:** Tkinter is included with most standard Python installations. On some Linux distributions, you may need to install the system package that provides Tkinter.

---

## 🎮 How to Play

1. Start the Python program.
2. The game board will open in a new window.
3. Click an empty square to place **X**.
4. The computer will automatically respond with **O**.
5. Continue playing until:

   * You win 🏆
   * The computer wins 🤖
   * The board becomes full and the game ends in a draw 🤝
6. Click **🔄 Restart Game** to start a new match.

---

## 🔍 Main Components

### `check_winner()`

Checks all possible winning combinations:

* Horizontal rows
* Vertical columns
* Main diagonal
* Opposite diagonal

It returns the winning player when a winning combination is found.

### `is_full()`

Checks whether all nine board positions are occupied.

If there are no empty cells and nobody has won, the game is declared a draw.

### `minimax()`

This is the core of the AI.

It recursively explores possible future moves and evaluates the resulting game states.

The AI tries to maximize its score, while the player is treated as an opponent attempting to minimize that score.

### `best_move()`

Tests the available moves for the computer and selects the move with the highest Minimax score.

### `player_move()`

Handles the player's button click, updates the board with `X`, and checks whether the player has won or the game has ended in a draw.

### `ai_turn()`

Calculates the computer's best move using Minimax and places `O` on the selected square.

### `reset_game()`

Clears the board and enables all buttons so that a new game can be played.

---

## 📸 Screenshots

Add screenshots of the game here after running the application.

Example:

```text
screenshots/
├── game-board.png
├── player-win.png
└── computer-win.png
```

You can then display them in this section:

```markdown
![Game Board](screenshots/game-board.png)
```

---

## 📚 Concepts Demonstrated

This project demonstrates several important programming and computer-science concepts:

* Python functions
* Recursion
* Conditional statements
* Loops
* Lists and arrays
* Event-driven programming
* Graphical User Interfaces
* Game-state representation
* Artificial Intelligence
* Adversarial search
* Minimax decision making
* Basic algorithmic problem solving

---

## 🔮 Future Improvements

Possible improvements for future versions include:

* [ ] Add difficulty levels
* [ ] Add player name input
* [ ] Add score tracking
* [ ] Add Player vs Player mode
* [ ] Add Player vs AI mode selection
* [ ] Improve the graphical design
* [ ] Add sound effects
* [ ] Add game statistics
* [ ] Add an AI difficulty system
* [ ] Add a game history
* [ ] Add an option for the player to choose X or O

---

## 👨‍💻 Author

**Mrmanticore**

GitHub:
https://github.com/Mrmanticore

---

## 📄 License

This project is available for educational and personal use.

If you add a formal open-source license to the repository, update this section to match the license you choose.
