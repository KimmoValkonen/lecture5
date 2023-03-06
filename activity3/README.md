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
# A: They differ in their approach and the types of problems they are best suited for. 
- State some application of dynamic programming
# A:
- Make a change problem
- Knapsack problem
- Optimal binary search tree

- Difference between recursion vs dynamic programming
# A:
In dynamic programming, problems are solved by breaking them down into smaller ones to solve the larger ones, while recursion is when a function is called and executed by itself. While dynamic programming can function without making use of recursion techniques, since the purpose of dynamic programming is to optimize and accelerate the process, programmers usually make use of recursion techniques to accelerate and turn the process efficiently.
When a function can execute a specific task by calling itself, receive the name of the recursive function. In order to perform and accomplish the work, this function calls itself when it has to be executed.
Using dynamic programming, you can break a problem into smaller parts, called subproblems, to solve it. Dynamic programming involves solving the problem for the first time, then using memoization to store the solutions.
Therefore, the main difference between the two techniques is their intended use; recursion is used to automate a function, whereas dynamic programming is an optimization technique used to solve problems.
Recursive functions recognize when they are needed, execute themselves, then stop working. When the function identifies the moment it is needed, it calls itself and is executed; this is called a recursive case. As a result, the function must stop once the task is completed, known as the base case.
By establishing states, dynamic programming recognizes the problem and divides it into sub-problems in order to solve the whole scene. After solving these sub-problems, or variables, the programmer must establish a mathematical relationship between them. Last but not least, these solutions and results are stored as algorithms, so they can be accessed in the future without having to solve the whole problem again.

- Difference between Top down and bottom up approaches to dynamic programming
1. Top-Down:
Break down the given problem in order to begin solving it. If you see that the problem has already been solved, return the saved answer. If it hasn’t been solved, solve it and save it. This is usually easy to think of and very intuitive.
2. Bottom-Up:
Analyze the problem and see in what order the subproblems are solved, and work your way up from the trivial subproblem to the given problem. This process ensures that the subproblems are solved before the main problem.

- How to solve a Dynamic Programming Problem?
# A: Steps to solve a Dynamic programming problem:
- Identify if it is a Dynamic programming problem.
- Decide a state expression with the Least parameters.
- Formulate state and transition relationships.
- Do tabulation (or memorization).

> Refer to the [links](#links) section below

## Links

- https://cpp.sh/
- [Recursion vs dynamic programming](https://www.geeksforgeeks.org/introduction-to-dynamic-programming-data-structures-and-algorithm-tutorials/)
- [How to solve a Dynamic Programming Problem ?](https://www.geeksforgeeks.org/solve-dynamic-programming-problem/)
