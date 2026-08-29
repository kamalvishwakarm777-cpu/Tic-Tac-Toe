# 🎮 Tic-Tac-Toe Game in Java

A simple **Tic-Tac-Toe game built using Java and Object-Oriented Programming (OOP) principles**.

This project was created to strengthen my understanding of how OOP concepts can be applied to a real-world problem. Instead of writing the complete game logic in a single class, the application is designed by separating responsibilities into different classes and objects.

---

## 📌 About the Project

Tic-Tac-Toe is a classic two-player game played on a **3 × 3 board**.

Players take turns placing their symbol:

* ❌ Player 1 → `X`
* ⭕ Player 2 → `O`

The player who successfully places three of their symbols in a horizontal, vertical, or diagonal line wins the game.

This project focuses not only on implementing the game logic but also on understanding how **Object-Oriented Programming** helps in designing clean, maintainable, and scalable applications.

---

## 🚀 Features

* 🎮 Two-player gameplay
* 🔄 Alternate turns between players
* 🏆 Automatic winner detection
* 🤝 Draw detection
* ❌ Invalid move handling
* 🔁 Option to restart the game
* 🧩 Clean object-oriented design
* 📚 Practical implementation of Java OOP concepts

---

## 🧠 OOP Concepts Used

This project helped me understand how Object-Oriented Programming can be applied to a real problem.

### 1. Encapsulation 🔒

Each class manages its own data and behavior.

For example:

* The `Board` class handles the game board.
* The `Player` class stores player information.
* The `Game` class controls the overall game flow.

This prevents unnecessary access to internal data and keeps the code organized.

---

### 2. Abstraction 🎭

The game hides complex implementation details behind simple methods.

For example:

```java
board.makeMove(row, column, symbol);
```

The user of this method does not need to know how the board internally stores or validates the move.

---

### 3. Inheritance 🧬

Inheritance can be used to create specialized types of players.

For example:

```text
Player
 ├── HumanPlayer
 └── ComputerPlayer
```

This allows different player types to share common properties and behavior.

---

### 4. Polymorphism 🔄

Different types of players can implement their own version of making a move.

For example:

```java
player.makeMove();
```

The behavior can change depending on whether the player is:

* A Human Player
* A Computer Player

This makes the application more flexible and easier to extend.

---

## 🏗️ Project Structure

```text
TicTacToe/
│
├── src/
│   │
│   ├── Main.java
│   ├── Game.java
│   ├── Board.java
│   ├── Player.java
│   └── ...
│
├── README.md
└── .gitignore
```

> The exact structure may vary depending on the implementation.

---

## 🎯 Class Responsibilities

### `Player`

Responsible for storing player-related information.

Possible attributes:

* Player name
* Player symbol (`X` or `O`)

Possible behavior:

* Make a move
* Get player details

---

### `Board`

Responsible for managing the Tic-Tac-Toe board.

Possible responsibilities:

* Display the board
* Validate moves
* Place symbols
* Check available positions
* Check winning conditions
* Check for a draw

---

### `Game`

Responsible for controlling the overall game.

Possible responsibilities:

* Start the game
* Manage player turns
* Accept player moves
* Check game status
* Declare the winner
* Handle game restart

---

### `Main`

The entry point of the application.

Responsible for:

* Creating game objects
* Starting the game

---

## 🔄 Game Flow

```text
Start Game
    │
    ▼
Create Players
    │
    ▼
Initialize Board
    │
    ▼
Player 1 Turn
    │
    ▼
Validate Move
    │
    ▼
Update Board
    │
    ▼
Check Winner
    │
 ┌──┴──┐
 │     │
Yes    No
 │      │
 ▼      ▼
Winner  Check Draw
 │        │
 │     ┌──┴──┐
 │     │     │
 │    Yes    No
 │     │      │
 ▼     ▼      ▼
End    Draw  Next Player
Game         │
             └──────►
```

---

## 💡 Why OOP for Tic-Tac-Toe?

Without OOP, the entire game could be written inside a single `main()` method.

However, as the project grows, this approach becomes difficult to manage.

Using OOP allows us to divide the application into meaningful objects:

| Object | Responsibility             |
| ------ | -------------------------- |
| Player | Represents a player        |
| Board  | Represents the game board  |
| Game   | Controls the game          |
| Move   | Represents a player's move |

This makes the code:

* Easier to understand
* Easier to maintain
* Easier to test
* Easier to extend

---

## 🔮 Possible Future Improvements

Some features that can be added in the future:

* 🤖 Computer AI player
* 🖥️ Graphical User Interface (GUI)
* 🌐 Multiplayer support
* 🧠 Minimax algorithm for unbeatable AI
* 💾 Save game functionality
* 📊 Scoreboard
* ⏱️ Timer for each player
* 🎨 Improved UI using JavaFX or Swing

---

## 🛠️ Technologies Used

* **Java**
* **Object-Oriented Programming**
* **Java Collections** *(if used)*
* **Scanner for user input**
* **IDE:** IntelliJ IDEA / Eclipse / VS Code

---

## ▶️ How to Run

### Clone the repository

```bash
git clone <your-repository-url>
```

### Navigate to the project directory

```bash
cd TicTacToe
```

### Compile the project

```bash
javac src/*.java
```

### Run the application

```bash
java Main
```

> Update the commands according to your project structure and package configuration.

---

## 📚 What I Learned

Through this project, I gained a better understanding of:

* Object-Oriented Programming
* Class and Object design
* Encapsulation
* Abstraction
* Inheritance
* Polymorphism
* Separation of responsibilities
* Game logic implementation
* Input validation
* Writing clean and maintainable Java code

---

## 🎓 Key Takeaway

> **OOP is not just about creating classes. It is about identifying real-world entities, assigning responsibilities, and allowing objects to interact with each other in a clean and structured way.**

Building this Tic-Tac-Toe game helped me understand how a real-world problem can be broken down into objects and responsibilities using Object-Oriented Programming.

---

## 🤝 Contributions

Contributions, suggestions, and improvements are welcome!

Feel free to:

* Fork this repository
* Create a new branch
* Make your changes
* Submit a pull request

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

---

### 👨‍💻 Author

**Your Name**

Built with ❤️ using Java and OOP principles.
