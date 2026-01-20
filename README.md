# Tic-Tac-Toe – Low Level Design (LLD)

A clean, object-oriented implementation of the classic **Tic-Tac-Toe** game, designed with extensibility, testability, and interview-readiness in mind.  
This project focuses on **Low-Level Design (LLD)** principles rather than UI, making it ideal for system design discussions and OOP practice.


## 📌 Overview

Tic-Tac-Toe is a two-player game played on a **3×3 grid** where players take turns placing their symbols (**X** or **O**).  
The goal is to place **three identical symbols in a row**, column, or diagonal.  
If the board fills up with no winner, the game ends in a **draw**.

This design supports:
- Player vs Player mode
- Move validation
- Winner & draw detection
- Persistent scoreboard across games
- Clean separation of concerns using design patterns


## 🎯 Requirements

### Functional Requirements
- 3×3 game board
- Two players (X and O) take alternate turns
- Reject invalid moves (cell already filled)
- Detect and announce:
  - Winner
  - Draw
- Maintain a scoreboard across multiple games
- Game flow simulated via a driver/demo class

### Non-Functional Requirements
- Strong Object-Oriented Design
- Modular and extensible architecture
- Easy to test and maintain
- Clear console output for board state


## 🧱 Core Entities

| Entity | Responsibility |
|------|----------------|
| **Board** | Manages the grid and win/draw logic |
| **Cell** | Represents a single grid position |
| **Player** | Represents a player with a symbol |
| **Symbol (enum)** | X, O, EMPTY |
| **Game** | Controls gameplay flow |
| **GameStatus (enum)** | IN_PROGRESS, WINNER_X, WINNER_O, DRAW |
| **Scoreboard** | Tracks wins and draws |
| **TicTacToeSystem** | Orchestrates games and scoreboard |


## 🏗️ Class Design

### Enums
Symbol      → X, O, EMPTY
GameStatus  → IN_PROGRESS, WINNER_X, WINNER_O, DRAW
