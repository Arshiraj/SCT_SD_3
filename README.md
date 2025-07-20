# SCT_SD_3
#  Sudoku Solver in C++

This project is a **Sudoku solver** written in C++ using **backtracking algorithm**. It takes a 9x9 Sudoku grid as input with empty cells represented by `0`, and solves the puzzle if a valid solution exists.

---

## ✅ Features

- Solves standard 9x9 Sudoku puzzles
- Uses backtracking algorithm for recursive solution
- Clean console output of both input and solved Sudoku grids

---

## 📂 Files

- `sudoku_solver.cpp` – Main source code file
- You can run this file with any C++ compiler like `g++`.

---

## 🧠 How It Works

1. The `solveSudoku()` function tries to fill empty cells with numbers from 1 to 9.
2. For each number, it checks if placing it is safe:
   - Not already in the same row
   - Not already in the same column
   - Not already in the 3x3 subgrid
3. If a valid number is found, it fills the cell and recursively tries to solve the rest of the grid.
4. If stuck, it backtracks and tries the next number.

---


Sample Input:-
Input Puzzle:
5 1 7 6 0 0 0 3 4
2 8 9 0 0 4 0 0 0
3 4 6 2 0 5 0 9 0
6 0 2 0 0 0 0 1 0
0 3 8 0 0 6 0 4 7
0 0 0 0 0 0 0 0 0
0 9 0 0 0 0 0 7 8
7 0 3 4 0 0 5 6 0
0 0 0 0 0 0 0 0 0


output:-
Solved Puzzle:
5 1 7 6 9 8 2 3 4
2 8 9 1 3 4 7 5 6
3 4 6 2 7 5 8 9 1
6 7 2 8 4 9 3 1 5
1 3 8 5 2 6 9 4 7
9 5 4 7 1 3 6 8 2
4 9 5 3 6 2 1 7 8 
7 2 3 4 8 1 5 6 9
8 6 1 9 5 7 4 2 3


