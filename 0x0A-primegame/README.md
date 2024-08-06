# 0x0A. Prime Game

## Overview

This project involves solving a competitive game scenario where players strategically remove prime numbers and their multiples from a set of consecutive integers. The game tests your understanding of prime numbers, game theory, and algorithm optimization.

## Concepts Needed

### Prime Numbers
- **Definition**: Prime numbers are natural numbers greater than 1 that have no positive divisors other than 1 and themselves.
- **Identification**: Efficient algorithms to identify prime numbers within a given range are crucial for this game.

### Sieve of Eratosthenes
- **Algorithm**: This is an efficient algorithm to find all prime numbers up to a specified integer. It works by iteratively marking the multiples of each prime number starting from 2.
- **Importance**: Essential for precomputing prime numbers for each round of the game.

### Game Theory
- **Competitive Games**: Understanding the principles of games where two players take turns and the concept of optimal play.
- **Win Conditions**: Identifying strategies that lead to a win or loss.

### Dynamic Programming/Memoization
- **Optimization**: Using previous results to speed up future calculations, which is vital for handling multiple rounds efficiently.

### Python Programming
- **Control Structures**: Using loops and conditional statements to implement game logic and algorithms.
- **Data Structures**: Arrays and lists for storing the integers and tracking the removal of numbers.

## Project Requirements

- **Environment**: Ubuntu 20.04 LTS, Python 3.4.3
- **Code Style**: PEP 8
- **Execution**: All files must be executable and end with a new line.
- **Shebang**: The first line of all your files should be `#!/usr/bin/python3`.
- **No Imports**: You cannot import any packages.

## Tasks

### 0. Prime Game

Maria and Ben play a game where they take turns choosing a prime number from a set of consecutive integers starting from 1 up to and including `n`. They then remove that number and its multiples from the set. The player who cannot make a move loses the game.

- **Function Prototype**: `def isWinner(x, nums)`
  - **Parameters**:
    - `x`: The number of rounds.
    - `nums`: An array of integers representing the upper limit of the set of consecutive integers for each round.
  - **Returns**: The name of the player who won the most rounds. If the winner cannot be determined, return `None`.

#### Example

```python
x = 3
nums = [4, 5, 1]
```

1. **First Round (n = 4)**
   - Maria picks 2 and removes 2, 4, leaving [1, 3].
   - Ben picks 3 and removes 3, leaving [1].
   - Ben wins because there are no prime numbers left for Maria.

2. **Second Round (n = 5)**
   - Maria picks 2 and removes 2, 4, leaving [1, 3, 5].
   - Ben picks 3 and removes 3, leaving [1, 5].
   - Maria picks 5 and removes 5, leaving [1].
   - Maria wins because there are no prime numbers left for Ben.

3. **Third Round (n = 1)**
   - Ben wins because there are no prime numbers for Maria to choose.

Result: Ben wins 2 rounds, Maria wins 1 round. Ben is the overall winner.

## Additional Resources

- **Prime Numbers and Sieve of Eratosthenes**:
  - [Khan Academy: Prime Numbers](https://www.khanacademy.org/math/algebra/x2f8bb11595b61c86:quadratic-functions/x2f8bb11595b61c86:intro-to-prime-numbers/v/introduction-to-prime-numbers)
  - [Sieve of Eratosthenes in Python](https://www.geeksforgeeks.org/sieve-of-eratosthenes/)

- **Game Theory Basics**:
  - [Game Theory Introduction](https://www.investopedia.com/terms/g/gametheory.asp)

- **Dynamic Programming**:
  - [What Is Dynamic Programming With Python Examples](https://realpython.com/dynamic-programming/)

- **Python Official Documentation**:
  - [Python Lists](https://docs.python.org/3/tutorial/datastructures.html)

By understanding these concepts and utilizing the recommended resources, you will be well-prepared to solve the problem efficiently. The key to success is applying efficient algorithms to manage the game state and making optimal decisions based on the game's rules.

## Repository

- **GitHub Repository**: [alx-interview](https://github.com/paschalugwu/alx-interview)
- **Directory**: `0x0A-primegame`
- **File**: `0-prime_game.py`

## License

© 2024 ALX, All rights reserved.
