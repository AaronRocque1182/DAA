
# DAA (TA1) - Travelling Salesman Problem 

Given a set of nodes and distances as well as time taken to travel between every pair of nodes, the problem is to find the shortest possible path that visits every node exactly once and returns to the starting point, such that:

1. The path has the Least Distance Cost
2. The path has the Least Time Cost 
3. The path has a Decent Distance and Time Cost


## Explanation

Travelling salesman problem is the most notorious computational problem. We can use brute-force approach to evaluate every possible tour and select the best one. For n number of vertices in a graph, there are (n - 1)! number of possibilities.

Instead of brute-force using dynamic programming approach, the solution can be obtained in lesser time, though there is no polynomial time algorithm.

Let us consider a graph G = (V, E), where V is a set of cities and E is a set of weighted edges. An edge e(u, v) represents that vertices u and v are connected. Distance between vertex u and v is d(u, v), which should be non-negative.

Suppose we have started at city 1 and after visiting some cities now we are in city j. Hence, this is a partial tour. We certainly need to know j, since this will determine which cities are most convenient to visit next. We also need to know all the cities visited so far, so that we don't repeat any of them. Hence, this is an appropriate sub-problem.








## Test Case-1

double[][][] matrix = \
{ { { 0, 0 }, { 10, 15 }, { 15, 4 }, { 20, 7 } }, \
{ { 5, 13 }, { 0, 0 }, { 9, 3 }, { 10, 2 } }, \
{ { 6, 10 }, { 13, 10 }, { 0, 0 }, { 12, 9 } }, \
{ { 8, 14 }, { 8, 15 }, { 9, 16 }, { 0, 0 } } }; 

![Screenshot (45)](https://user-images.githubusercontent.com/107600168/192852849-15f4502d-3ef8-45cd-9fb3-e25fa1d38174.png)

## Test Case-2

double[][][] matrix = \
{ { { 0, 0 }, { 15, 20 }, { 25, 14 }, { 25, 12 } }, \
{ { 10, 18 }, { 0, 0 }, { 14, 8 }, { 15, 7 } }, \
{ { 11, 15 }, { 18, 15 }, { 0, 0 }, { 17, 14 } }, \
{ { 13, 19 }, { 13, 18 }, { 14, 21 }, { 0, 0 } } };

![Screenshot (46)](https://user-images.githubusercontent.com/107600168/192853996-aebe5245-5e70-496e-b00f-f3e8bd8ee896.png)

## Author

- [@AaronRocque1182](https://github.com/AaronRocque1182)


