# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

- I learned how to use and integrate backtracking, propagation within constraints, and DFS and BFS. I had challenges updating the board with the correct possibilities and making sure that `find_most_constrained_cell` found the right cell. Another challenge was the `failure_test` and `goal_test` and make sure they didn't fail or return the wrong thing.



2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

You could use the searching through possibilities, making decisions, and backtracking for things such as scheduling workers, resource allocation, and another type of puzzle game. DFS can be used for when the solution is deep inside the game and BFS can be used when the solution is short such as in finding the quickest route between 2 points. I learned about breaking a big problem into a smaller problem in coding solutions, such as the big Sodoku to the grids inside of it.

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

A stack and queue are data structures used to organize the data we have. The stack for last in first out can be seen as a pile of paper. You add with `push` and put it at the top and remove with `pop`. Queue is  for first in first out and can be seen as a line where you queue in and then queue out.