# Activities

## Task 1

Refer to the following link. Explain how the Knapsack Algorithm works:
https://monicagranbois.com/knapsack-algorithm-visualization/

## A: Dynamic programming breaks the problem into subproblems. The solution to each subproblem is stored and used to solve other, larger, subproblems. The final solution is built up from these subproblems.

In this case, an in-memory table stores the max value at different weights and number of items. Those values are used to build up a table that last's cell will contain the max value the knapsack can contain. The algorithm then walks through the table to get the items that make up that max value.

## Task 2

Refer to the following link. What are the difference between the brute force and the optimized solutions to the Knapsack problem.
https://www.educative.io/blog/0-1-knapsack-problem-dynamic-solution

# Answer
Brute force:
- Time complexity: O(2n), due to the number of calls with overlapping subcalls.
- Auxiliary space: O(1), no additional storage is needed.

Optimized:
- Time complexity: O(N∗C), our memoization table stores results for all subproblems and will have a maximum of N∗C subproblems.
- Auxiliary space: O(N∗C+N), O(N∗C) space for the memoization table, and O(N) space for recursion call-stack.

## Task 3

There are different implementations of the stair case problem in the following link:
https://www.enjoyalgorithms.com/blog/climbing-stairs-problem

Compare the time and space complexity of the different approaches

## Task 4: Individual (at home)

- Difference between divide and conquer and dynamic programming
- State some application of dynamic programming
- Difference between recursion vs dynamic programming
- Difference between Top down and bottom up approaches to dynamic programming
- How to solve a Dynamic Programming Problem?

> Refer to the [links](#links) section below

## Links

- https://cpp.sh/
- [Recursion vs dynamic programming](https://www.geeksforgeeks.org/introduction-to-dynamic-programming-data-structures-and-algorithm-tutorials/)
- [How to solve a Dynamic Programming Problem ?](https://www.geeksforgeeks.org/solve-dynamic-programming-problem/)
