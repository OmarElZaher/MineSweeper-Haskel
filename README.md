# Haskell Minesweeper Solver

## Overview

This repository contains a Haskell implementation designed to solve a Minesweeper-like game. The project utilizes functional programming principles in Haskell to navigate through a grid, perform specific actions on cells, and ultimately solve the game by reaching the end goal.

---

## Code Structure

### Data Types
- `Cell`: Represents coordinates on the grid.
- `MyState`: Represents the state of the game, including current cell, a list of remaining cells, string actions, and previous state.

### Functions

- **Navigation Functions**:
  - `up`: Move the current cell up.
  - `down`: Move the current cell down.
  - `left`: Move the current cell left.
  - `right`: Move the current cell right.
  
- **Utility Functions**:
  - `collect`: Collects a cell if it matches the current coordinates.
  - `nextMyStates`: Generates possible next states based on current state.

- **Search & Solve Functions**:
  - `isGoal`: Determines if the current state is the goal state.
  - `search`: Performs a search to find the goal state.
  - `constructSolution`: Constructs the solution string based on the found goal state.
  - `solve`: Entry point to initiate the solver.

---

## Usage

To execute the solver, use the `solve` function, providing the starting cell coordinates and a list of cells to navigate:

\`\`\`haskell
solve (startX, startY) listOfCells
\`\`\`

This function will generate a list of actions required to solve the Minesweeper-like game.

---

## How It Works

1. **Initialization**: Start with a grid containing cells.
2. **State Transition**: Utilize navigation functions to explore the grid, collect cells, and progress towards the goal.
3. **Search Algorithm**: Implement a search mechanism to determine the optimal path and actions to solve the game.
4. **Solution Construction**: Generate a list of strings representing actions to solve the game.

---

## Contributions

We welcome contributions to enhance the solver, improve efficiency, or add additional functionalities. Please fork the repository, implement your changes, and submit a pull request for review.

---

## Acknowledgments

Special thanks to the Haskell community for fostering a vibrant ecosystem and enabling the development of this Minesweeper solver using functional programming paradigms.

---

For any inquiries or suggestions, please feel free to reach out to the repository maintainers.
