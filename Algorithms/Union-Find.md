# Union Find

Union Find is an algorithm for solving dynamic connectivity, percolation, Games with large search spaces, least common ancestor problems, and others. With 10^9 operations on 10^9 options it would take 30 years to solve. Because it's time complexity is O(n^2) (quadratic) it won't scale up with better compute. However with simple algorithmic improvements such as weighting and path compression, you can speed that time up to 6 seconds, with a final worst-case time complexity of N + M lg* N
