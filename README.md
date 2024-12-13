# Vertux_Vertusa
This project focuses on implementing algorithms to find the Maximal Independent Set (MIS) of vertices in a graph. The Maximal Independent Set is a subset of vertices such that no two vertices in the set are adjacent, and no additional vertices can be added without breaking this property.

**Brute Force Approach for MIS(Minimum Independent Set)**
The brute force approach for finding the maximal independent set (MIS) involves
checking every possible subset of vertices and determining which of these subsets
forms an independent set. Among all valid independent sets, we select the largest one.
**Steps for Brute Force Algorithm:**
1. Generate all possible subsets of vertices.
2. Check each subset to see if it forms an independent set (i.e., no two vertices in
the subset are connected by an edge).
3. Keep track of the largest independent set.
4. Return the maximal independent set.

**Greedy Approximation Algorithm**
One of the simplest approximation algorithms for finding an independent set is the
greedy algorithm.
**Algorithm (Greedy Approximation):**
1. Initialize an empty set: Start with an empty set SSS to store the independent set.
2. Sort vertices by degree: Sort all vertices based on some heuristic (commonly by
degree, i.e., the number of edges connected to the vertex).
3. Iterate over vertices: For each vertex v:
o If v is not adjacent to any vertex already in the independent set SSS, add vvv
to SSS.
4. Continue until no more vertices can be added.
5. Return the set: The set SSS is the approximate independent set.
Example:
• Start with an empty set S=∅.
• Sort vertices by degree (or use a random order).
• Add the first vertex to SSS, and then skip any vertices adjacent to this vertex.
• Continue until all vertices are considered.
