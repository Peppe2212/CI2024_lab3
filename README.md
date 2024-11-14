# CI2024_lab3

The 8-puzzle problem is a classic sliding puzzle consisting of a 3x3 grid with eight numbered tiles and one empty space. The objective is to move the tiles around by sliding them into the empty space to reach a specific goal configuration, typically in ascending order from 1 to 8 with the empty space in the bottom-right corner.

In this lab is implemented the A* algorithm, considered one of the best algorithm to solve this problem. The A* is implemented using the heuristic of the Manhattan Distance, which is also one of the better heuristic for this problem.

The A* presented in the code use heap as a priority queue, it is used for taking the best node. Where the best node is the one that assume the minimum cost (influenced by the heuristic), so following: 

$$
f(n) = g(n) + h(n)
$$

where f(n) is the total cost, g(n) is the cost for reach that node and h(n) is the distance to the node calculated by the heuristic (in this application is the Manhattan distance).



#### Why the A* and not a Depth-First Search?
 The branching factor is quite high, so DFS risks running out of memory quickly, in one other hand is important to choose a correct heuristic for A*.

A* in general is more performing because is developed for finding the best path looking only the action that seems good, differently the DFS explore in deep without take care of cost or a strategy for finding the final state quicker as possible. For that, for this problem is not very performing.

