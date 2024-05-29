# Pascal's Triangle Project

This project focuses on implementing a function in Python that generates Pascal's Triangle, a classic algorithmic problem that demonstrates key concepts in programming such as loops, list comprehensions, and basic arithmetic operations.

## Table of Contents
- [Project Overview](#project-overview)
- [Resources](#resources)
- [Must Know Concepts](#must-know-concepts)
- [Task](#task)
- [Usage](#usage)
- [Repository Structure](#repository-structure)

## Project Overview

In this project, you will create a function `pascal_triangle(n)` that returns a list of lists of integers representing Pascal’s Triangle up to the nth row.

## Resources

- [What is Pascal’s triangle](https://en.wikipedia.org/wiki/Pascal%27s_triangle)
- [Pascal’s Triangle - Numberphile](https://www.youtube.com/watch?v=XMriWTvPXHI)
- [What are Python Algorithms](https://realpython.com/python-algorithms/)

### Additional Resources

- [Mock Technical Interview](https://www.interviewbit.com/mock-interview/)

## Must Know Concepts

To successfully complete this project, you should revise the following Python concepts:

- **Lists and List Comprehensions:**
  - Create, access, modify, and iterate over lists.
  - Utilize list comprehensions for generating rows of Pascal’s Triangle.
- **Functions:**
  - Define and call functions.
  - Pass parameters and return values, particularly lists of lists representing Pascal’s Triangle.
- **Loops:**
  - Use `for` and `while` loops to iterate through sequences.
  - Implement nested loops for generating rows and calculating values in Pascal’s Triangle.
- **Conditional Statements:**
  - Apply `if`, `elif`, and `else` conditions for logic implementation.
- **Recursion (Optional):**
  - Understand recursion as an alternative approach.
  - Recognize base cases and recursive cases.
- **Arithmetic Operations:**
  - Perform addition for calculating elements of Pascal’s Triangle.
- **Indexing and Slicing:**
  - Access elements and slices of lists.
- **Memory Management:**
  - Understand how lists are stored and copied.
- **Error and Exception Handling (Optional):**
  - Use `try-except` blocks for handling errors.
- **Efficiency and Optimization:**
  - Consider time and space complexity.
  - Apply optimizations to improve performance.

## Task

### 0. Pascal's Triangle

Create a function `def pascal_triangle(n):` that returns a list of lists of integers representing the Pascal’s triangle of `n`:

- Returns an empty list if `n <= 0`.
- You can assume `n` will always be an integer.

```python
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))

if __name__ == "__main__":
    print_triangle(pascal_triangle(5))
```

Example output:
```
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
```

## Usage

To test the function, run the following command:
```bash
./0-main.py
```

## Repository Structure

- **Repository:** `alx-interview`
- **Directory:** `0x00-pascal_triangle`
- **File:** `0-pascal_triangle.py`
