# Lockboxes Project

## Overview

The Lockboxes project is a fascinating algorithmic challenge that requires the application of various concepts in computer science, particularly in graph theory and data structures. This README provides an explanation of the task, necessary concepts, and resources to help you develop an efficient solution.

## Project Description

You have a set of `n` locked boxes, each numbered from `0` to `n-1`. Each box may contain keys that can unlock other boxes. Your task is to write a method that determines if all the boxes can be opened, starting with the first box (box `0`), which is already unlocked.

### Task Requirements

- **Prototype**: `def canUnlockAll(boxes)`
- `boxes` is a list of lists, where each sublist represents the keys contained in a particular box.
- A key with the same number as a box can open that box.
- Assume all keys are positive integers.
- There may be keys that do not correspond to any box.
- The first box, `boxes[0]`, is always unlocked.
- The method should return `True` if all boxes can be opened, otherwise `False`.

### Example

```python
boxes = [[1], [2], [3], [4], []]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
print(canUnlockAll(boxes))  # Output: False
```

## Concepts and Resources

To solve this problem efficiently, you'll need to understand the following key concepts:

### Lists and List Manipulation
Understanding how to work with lists in Python, including accessing elements, iterating over lists, and modifying lists dynamically, is crucial.

- **Resource**: [Python Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)

### Graph Theory Basics
The boxes and keys can be conceptualized as nodes and edges in a graph. Knowledge of graph traversal algorithms, such as Depth-First Search (DFS) and Breadth-First Search (BFS), is very helpful.

- **Resource**: [Graph Theory](https://www.khanacademy.org/computing/computer-science/algorithms#graph-representation)

### Algorithmic Complexity
Understanding time and space complexity can help in writing more efficient algorithms. You'll want to analyze and optimize the complexity of your solution.

- **Resource**: [Big O Notation](https://www.geeksforgeeks.org/analysis-of-algorithms-set-1-asymptotic-analysis/)

### Recursion
Some solutions might involve a recursive approach to traverse through the boxes and keys.

- **Resource**: [Recursion in Python](https://realpython.com/python-recursion/)

### Queue and Stack
Using queues and stacks is crucial for implementing BFS or DFS algorithms, respectively, to traverse through the keys and boxes.

- **Resource**: [Python Queue and Stack](https://www.geeksforgeeks.org/stack-in-python/)

### Set Operations
Using sets to keep track of visited boxes and available keys can optimize the search process by avoiding duplicates and unnecessary checks.

- **Resource**: [Python Sets](https://docs.python.org/3/tutorial/datastructures.html#sets)

## Requirements

- **Editors**: vi, vim, emacs
- **Interpreter**: Python 3.4.3 on Ubuntu 20.04 LTS
- **Code Style**: PEP 8 (version 1.7.x)
- **Executable Files**: All files must be executable and end with a new line. The first line of all your files should be exactly `#!/usr/bin/python3`.

## Implementation

While the specific solution code is not provided here, the following steps outline the approach to develop your solution:

1. **Initialize**: Create a set to keep track of unlocked boxes and a list to use as a stack for DFS or a queue for BFS.
2. **Start with Box 0**: Begin from the first box, adding it to the unlocked set and its keys to the stack/queue.
3. **Traversal**: Use DFS/BFS to traverse through the keys and unlock subsequent boxes, adding newly found keys to the stack/queue.
4. **Check Completion**: After traversal, check if all boxes from 0 to n-1 are in the unlocked set.
5. **Return Result**: Return `True` if all boxes are unlocked, otherwise `False`.

## Example Usage

```python
#!/usr/bin/python3
canUnlockAll = __import__('0-lockboxes').canUnlockAll

boxes = [[1], [2], [3], [4], []]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
print(canUnlockAll(boxes))  # Output: True

boxes = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
print(canUnlockAll(boxes))  # Output: False
```

## Repository

- **GitHub Repository**: `alx-interview`
- **Directory**: `0x01-lockboxes`
- **File**: `0-lockboxes.py`

By following this guide and leveraging the provided resources, you will be well-prepared to implement an efficient solution to determine if all boxes can be unlocked. Happy coding!
