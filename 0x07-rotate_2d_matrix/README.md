# Rotate 2D Matrix

This project involves implementing an in-place algorithm to rotate an n x n 2D matrix by 90 degrees clockwise. The solution requires a solid understanding of matrix manipulation and in-place operations in Python.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Concepts](#concepts)
3. [Requirements](#requirements)
4. [Tasks](#tasks)
5. [Usage](#usage)
6. [Resources](#resources)

## Project Overview
In this project, you'll create a function `rotate_2d_matrix` that rotates a given n x n 2D matrix 90 degrees clockwise in place. The project is designed to help you practice matrix manipulation and improve your algorithmic thinking skills.

## Concepts

### Matrix Representation in Python
- **Lists of Lists**: A 2D matrix in Python is represented as a list of lists.
- **Access and Modify Elements**: Learn how to access and modify elements in a 2D matrix using indexing.

### In-place Operations
- **Minimize Space Complexity**: Perform operations without creating copies of the matrix, modifying the original matrix instead.

### Matrix Transposition
- **Swap Rows and Columns**: Transposing a matrix involves swapping rows with columns.
- **Step in Rotation**: Transposition is a key step in the process of rotating the matrix.

### Reversing Rows
- **Row Manipulation**: Reverse the order of elements in each row after transposition to achieve the 90-degree rotation.

### Nested Loops
- **Iteration**: Use nested loops to iterate through the matrix elements.
- **Element Modification**: Modify elements within the nested loops to transpose and reverse rows.

## Requirements
- **Editors**: Use `vi`, `vim`, or `emacs`.
- **Execution Environment**: Ubuntu 20.04 LTS with Python 3.8.10.
- **File Conventions**: All files should end with a new line and start with `#!/usr/bin/python3`.
- **Coding Style**: Adhere to `pycodestyle` (version 2.8.0).
- **Module Usage**: Do not import any external modules.
- **Documentation**: Document all modules and functions.
- **Executable Files**: Ensure all files are executable.

## Tasks

### Task 0: Rotate 2D Matrix
Rotate an n x n 2D matrix by 90 degrees clockwise in place.

**Function Prototype:**
```python
def rotate_2d_matrix(matrix):
    """
    Rotates the given n x n 2D matrix 90 degrees clockwise in place.

    Args:
    matrix (list of list of int): The n x n matrix to rotate.
    """
```

**Example Usage:**
```python
#!/usr/bin/python3
"""
Test 0x07 - Rotate 2D Matrix
"""
rotate_2d_matrix = __import__('0-rotate_2d_matrix').rotate_2d_matrix

if __name__ == "__main__":
    matrix = [
        [1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]
    ]

    rotate_2d_matrix(matrix)
    print(matrix)
```

**Expected Output:**
```
[[7, 4, 1],
 [8, 5, 2],
 [9, 6, 3]]
```

## Usage
1. Clone the repository:
    ```bash
    git clone https://github.com/paschalugwu/alx-interview.git
    ```
2. Navigate to the project directory:
    ```bash
    cd alx-interview/0x07-rotate_2d_matrix
    ```
3. Execute the test script:
    ```bash
    ./main_0.py
    ```

## Resources
- **Python Official Documentation**:
    - [Data Structures](https://docs.python.org/3/tutorial/datastructures.html)
    - [More on Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
- **GeeksforGeeks**:
    - [Inplace rotate square matrix by 90 degrees](https://www.geeksforgeeks.org/inplace-rotate-square-matrix-by-90-degrees/)
    - [Transpose a matrix in Single line in Python](https://www.geeksforgeeks.org/transpose-matrix-single-line-python/)
- **TutorialsPoint**:
    - [Python Lists](https://www.tutorialspoint.com/python/python_lists.htm)

By understanding these concepts and utilizing the provided resources, you will be able to approach the problem methodically, first transposing the matrix and then reversing each row to achieve a 90-degree clockwise rotation.
