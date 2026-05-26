# SCT_SD_03
A high-performance Sudoku puzzle solver implemented in C utilizing a recursive backtracking algorithm. Features a user-friendly CLI grid input and validation system. Built for Task 03 of the SkillCraft Technology internship.
# Automated Sudoku Solver (C Implementation)

## 📌 Project Overview
This project is an automated **Sudoku Puzzle Solver** written in **C**. It takes an unsolved $9 \times 9$ Sudoku grid from the user via the command line, validates the initial puzzle configuration, and automatically finds the solution using a recursive backtracking algorithm.

Developed as **Task 03** during my internship at **SkillCraft Technology**, this project showcases algorithmic depth, matrix manipulation, and recursion constraints.

## 🚀 Features
- **Dynamic CLI Input:** Accepts puzzle rows line-by-line using numbers for known digits and dots (`.`) or zeros (`0`) for blank cells.
- **Pre-Validation Check:** Validates the initial board to ensure it follows standard Sudoku rules before attempting to solve.
- **Backtracking Algorithm:** Employs an efficient recursive depth-first search (DFS) pattern to evaluate possibilities and backtrack when paths hit a dead end.
- **Formatted Grid Layout:** Outputs the original and solved states in a clean, human-readable ASCII bounding-box matrix grid.

## 🛠️ Key Technical Concepts Demonstrated
- **Multi-Dimensional Arrays:** Manages state transitions synchronously using separate tracking matrices (`original[9][9]` and `grid[9][9]`).
- **Recursive Backtracking:** Uses standard algorithmic rules to safely trial values from $1$ to $9$ across empty cells.
- **Sub-Grid Mathematical Constraints:** Isolates $3 \times 3$ sub-boxes via index partitioning to enforce strict block rules alongside standard horizontal/vertical line exclusions.

## 💻 How to Compile and Run
You can compile and execute this program in your local terminal using standard C tools (like `gcc`):

```bash
# Compile the program
gcc sudoku.c -o solver

# Run the executable
./solver
