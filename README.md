This is a readme for the next 8 months work to be put.

Lots of things on the way....

```Dynamic Programming```

Overlapping : To use memory to use the previous state results for upcoming states\
**For non overlapping subproblems the Memory usage doesn't happen resulting in Divide & Conquer instead e.g Merge sort and Quick Sort**
Subproblem : Recursive breakdown. <Requires base case and a recursive case that eventually hits the base case>\

Overlapping subproblem : Any recursive algorithm should solve the same problem over and over rather than generating new subproblem.

Optimal Substructure : To ensure use of Bellman Equation. The optimal substructure formation is critical and most often the "TOUGH" part of dp problems. In other words, it means solutions to an optimization problem can be obtained by the combination of optimal soultions to subproblems.

Steps:
Memoization
1. Design a base case and a recursion that will eventually hit the base case
2. Create a state dictionary that results of each of the small states that will give O(1) lookup for the newer states results.
The size of dictionary depends on the total number of states the problem has including the base case. [The dictionary can be either constructed dynamically or initialized at the very beginning(faster)]
3. Optimal substructure for now remember that : Minima of smaller problem will eventually lead to minima of the larger problem

Tabular
1. Use the previous results to calculate next. fib[n] = fib[n-1] + fib[n-2] ; fib[0] = 0 & fib[1] = 1

~Pretty neat and sophisticated code that is very appealing to look at but hard to generate or understand sometimes. The glory is much higher than average to the people coming up with these sort of algorithms but sacrifices readability if overtly optimized~

2. 



Shortest Path problem Analysis (after memoization)
 - The (s,v) for V number of vertices for the different possibilities for v
 - Time/Subproblem : The minimization problem is number of incoming edges E to eaach v vertex and total V vertices will have E edges as incoming edges. indegree(v) + 1 for each vertex and so for all vertices V sum up the indegree for each vertex + constant time making E(indegrees) + V(there are V constant time operations)
 - V+E is | (->vertex) for all V vertices = E. 
 Sum of (indegree(v) + 1) = O(V+E) --> Handshaking Lemma