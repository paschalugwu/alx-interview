## 0x08. Making Change

### Overview

This project addresses the classic coin change problem, a common exercise in dynamic programming and greedy algorithms. The goal is to determine the minimum number of coins required to make up a given amount, using a provided set of coin denominations. The project involves implementing an efficient algorithm that solves this problem, considering different strategies and their computational complexities.

### Key Concepts

1. **Greedy Algorithms:**
   - Greedy algorithms make a series of choices, each of which looks best at the moment, to find a solution.
   - While they are intuitive and can be efficient, they do not always produce the optimal solution for all instances of the coin change problem.

2. **Dynamic Programming:**
   - This approach involves breaking down the problem into simpler subproblems and solving them once, storing the results for future reference.
   - It is particularly useful when dealing with optimization problems and is often necessary when greedy algorithms fall short.

3. **Algorithmic Complexity:**
   - Understanding the time and space complexity of algorithms is crucial for ensuring efficiency, especially with large inputs.
   - The coin change problem has both a naive solution and more optimized ones, with the latter often necessary to meet performance constraints.

4. **Problem-Solving Strategies:**
   - The problem can be tackled using iterative or recursive approaches.
   - Each approach has its benefits and trade-offs, and the choice may depend on factors such as clarity, ease of implementation, and efficiency.

5. **Python Programming:**
   - Effective use of Python's features, such as list comprehensions, loops, and conditional statements, is essential for implementing the solution.
   - Following PEP 8 guidelines ensures code readability and maintainability.

### Resources

To assist in understanding and implementing the solution, the following resources are recommended:

- **Python Official Documentation:** For foundational knowledge on control flow, including loops and conditionals.
- **GeeksforGeeks Articles:**
  - "Coin Change | DP-7" for a comprehensive guide on the dynamic programming approach.
  - "Greedy Algorithm to find Minimum number of Coins" for insights into the greedy algorithm approach.
- **YouTube Tutorials:** Visual explanations and step-by-step guides on the dynamic programming solution to the coin change problem.

### Project Tasks

#### Task 0: Change Comes from Within

**Objective:** Implement a function `makeChange(coins, total)` that determines the fewest number of coins needed to meet a given amount total.

- **Parameters:**
  - `coins`: A list of integers representing the denominations of the coins available.
  - `total`: The target amount to be achieved using the coins.

- **Return Values:**
  - The function returns the fewest number of coins needed to achieve the `total`.
  - If the `total` is 0 or less, return 0.
  - If the `total` cannot be achieved with the given coins, return -1.

- **Assumptions:**
  - Each coin denomination is a positive integer.
  - There is an infinite supply of each coin denomination.

**Evaluation:** The solution's runtime efficiency will be assessed.

### Repository Structure

- **GitHub Repository:** `alx-interview`
- **Directory:** `0x08-making_change`
- **File:** `0-making_change.py`

### License

This project is licensed under the terms and conditions outlined by ALX.

By mastering these concepts and utilizing the recommended resources, you will be well-equipped to tackle the coin change problem, determining whether a greedy or dynamic programming approach is best suited to the task at hand.
