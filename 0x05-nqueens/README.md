# N Queens Problem

Welcome to the **N Queens Problem** project. This README will guide you through understanding and solving the classic N Queens problem using backtracking algorithms. 

## Overview

The **N Queens problem** is a well-known puzzle in computer science and mathematics. The goal is to place **N non-attacking queens** on an **N×N chessboard**. This means that no two queens can share the same row, column, or diagonal.

## Concepts

### 1. Backtracking Algorithms

Backtracking is a general algorithm for finding all (or some) solutions to computational problems, notably constraint satisfaction problems. It incrementally builds candidates to the solutions and abandons a candidate ("backtracks") as soon as it determines that the candidate cannot possibly lead to a valid solution.

**Key Points:**
- **Exploration:** Systematically searches for a solution by exploring all possible positions for queens.
- **Backtracking:** Reverts the last move if it leads to an invalid solution.

[Learn more about Backtracking Algorithms](https://en.wikipedia.org/wiki/Backtracking)

### 2. Recursion

Recursion involves a function calling itself to solve smaller instances of the same problem. In this project, recursion will help explore all potential configurations of the queens on the board.

**Key Points:**
- **Base Case:** Defines when to stop the recursion.
- **Recursive Case:** Defines how to break the problem into smaller parts.

[Introduction to Recursion in Python](https://www.learnpython.org/en/Recursion)

### 3. List Manipulations in Python

Lists are used to keep track of the positions of queens on the board. You'll need to create, update, and manipulate these lists efficiently.

**Key Points:**
- **Initialization:** Create an empty list to store queen positions.
- **Appending:** Add new positions.
- **Validation:** Check positions for conflicts.

[Python Lists Documentation](https://docs.python.org/3/tutorial/datastructures.html)

### 4. Python Command Line Arguments

You'll handle input using command-line arguments to specify the size of the chessboard (N). The `sys` module will be used to parse and validate these inputs.

**Key Points:**
- **Reading:** Capture arguments from the command line.
- **Validation:** Ensure the input is an integer greater than or equal to 4.

[Command Line Arguments in Python](https://docs.python.org/3/library/sys.html#sys.argv)

## Project Tasks

### 0. N Queens

#### Task Description
Write a Python program that solves the N Queens problem.

**Requirements:**
- **Usage:** `nqueens N`
- **Input Validation:**
  - Print `Usage: nqueens N` and exit with status `1` if the number of arguments is incorrect.
  - Print `N must be a number` and exit with status `1` if `N` is not an integer.
  - Print `N must be at least 4` and exit with status `1` if `N` is less than 4.
- **Output:**
  - Print every possible solution in the format `[[row, col], ...]`.
  - Solutions do not need to be printed in any specific order.
- **Module:** Only the `sys` module is allowed.

#### Example Usage
```sh
$ ./0-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
$ ./0-nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
```

## Requirements

- **Editors:** `vi`, `vim`, `emacs`
- **Environment:** Ubuntu 20.04 LTS, Python 3.4.3
- **Code Style:** Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide (version 1.7.*).
- **File Execution:** Ensure all files are executable.

## Repository

- **GitHub Repository:** `alx-interview`
- **Directory:** `0x05-nqueens`
- **File:** `0-nqueens.py`

## License

This project is licensed under the terms of the ALX © 2024 license.
