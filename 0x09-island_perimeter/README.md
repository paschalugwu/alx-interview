# 0x09. Island Perimeter

## Project Overview

This project involves solving a geometric problem within a grid context using algorithms, data structures (specifically matrices or 2D lists), and iterative or conditional logic. The goal is to calculate the perimeter of a single island in a grid, where the grid is represented by a 2D array of integers. This project will help reinforce your ability to manipulate data structures and apply logical reasoning to solve problems.

## Concepts Needed

### 2D Arrays (Matrices)
- **Accessing and Iterating:** Learn to navigate through adjacent cells (horizontally and vertically) in a 2D array.
- **Navigating Adjacent Cells:** Understand how to efficiently move through a grid to check neighboring cells.

### Conditional Logic
- **Cell Contribution:** Apply conditions to determine whether a cell contributes to the perimeter of the island.

### Counting Techniques
- **Edge Counting:** Develop a method to count the edges that contribute to the island’s perimeter.

### Problem-Solving Strategies
- **Problem Breakdown:** Identify land cells and calculate their contribution to the perimeter by breaking down the problem into smaller tasks.

### Python Programming
- **Nested Loops:** Use nested loops for iterating over grid cells.
- **Conditional Statements:** Use conditional statements to check the status of adjacent cells.

## Resources
- **Python Official Documentation:**
  - [Nested Lists](https://docs.python.org/3/tutorial/datastructures.html#nested-list-comprehensions): Understanding how to work with lists within lists in Python.
- **GeeksforGeeks Articles:**
  - [Python Multi-dimensional Arrays](https://www.geeksforgeeks.org/python-using-2d-arrays-lists-the-right-way/): A guide to working with 2D arrays in Python effectively.
- **TutorialsPoint:**
  - [Python Lists](https://www.tutorialspoint.com/python/python_lists.htm): Explains how to create, access, and manipulate lists in Python.
- **YouTube Tutorials:**
  - [Python 2D Arrays and Lists](https://www.youtube.com/watch?v=X9gL4lLtFdI): Video tutorials on handling 2D arrays in Python.

## Additional Resources
- **Mock Technical Interviews:** Practice problem-solving techniques and prepare for technical interviews.

## Requirements
- **Editors:** vi, vim, emacs
- **Environment:** Files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.4.3).
- **File Requirements:**
  - All files should end with a new line.
  - The first line of all files should be exactly `#!/usr/bin/python3`.
  - Follow PEP 8 style (version 1.7).
  - Do not import any modules.
  - All modules and functions must be documented.
  - All files must be executable.

## Task

### 0. Island Perimeter

**Objective:** Create a function `def island_perimeter(grid):` that returns the perimeter of the island described in the grid.

- **Grid Characteristics:**
  - `0` represents water.
  - `1` represents land.
  - Each cell is square, with a side length of 1.
  - Cells are connected horizontally/vertically (not diagonally).
  - The grid is rectangular, with its width and height not exceeding 100.
  - The grid is completely surrounded by water.
  - There is only one island (or none).
  - The island doesn’t have “lakes” (water inside that isn’t connected to the water surrounding the island).

**Example:**
```python
if __name__ == "__main__":
    grid = [
        [0, 0, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 1, 1, 0, 0],
        [0, 0, 0, 0, 0, 0]
    ]
    print(island_perimeter(grid))  # Output should be 12
```

**Repository:**
- **GitHub repository:** alx-interview
- **Directory:** 0x09-island_perimeter
- **File:** 0-island_perimeter.py

---

By understanding these concepts and utilizing the provided resources, you will be equipped to approach the problem methodically. This project not only tests your algorithmic thinking but also reinforces your ability to manipulate data structures and apply logical reasoning to solve problems.
