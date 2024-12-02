# Graph Theory and Dynamic Programming: 
## Graph Theory

Graphs are foundational structures in computer science and mathematics, representing relationships between entities. This guide covers:

- **Directed vs. Undirected Graphs**
- **Weighted vs. Unweighted Graphs**

---

### 1. Directed vs. Undirected Graphs

#### What are Graphs?
A graph consists of nodes (vertices) connected by edges. Graphs model diverse systems like social networks, transportation grids, and communication channels.

#### **Directed Graphs (Digraphs)**

**Definition**  
A directed graph has edges with specific directions, indicating a one-way relationship between vertices.

**Key Properties**  
- Edges are represented as ordered pairs `(u, v)`, where:
  - `u` is the source vertex.
  - `v` is the destination vertex.
- Edges are depicted with arrows.

**Examples**  
- **Social Media**: A directed edge `(A, B)` indicates user A follows user B (e.g., Twitter).  
- **Road Networks**: A one-way street from A to B.

**Use Cases**  
- **Task Scheduling**: Represent dependencies between tasks.  
- **Data Flow Analysis**: Track dependencies in compilers or networks.

---

#### **Undirected Graphs**

**Definition**  
An undirected graph has edges without direction, representing mutual relationships between vertices.

**Key Properties**  
- Edges are represented as unordered pairs `{u, v}`, where `u` and `v` are equally connected.
- Connections are depicted as simple lines.

**Examples**  
- **Friendship Networks**: If A is connected to B, then B is also connected to A (e.g., Facebook).  
- **Utility Networks**: Represent electrical or water systems.

**Use Cases**  
- **Network Design**: Simulating transportation or utility systems.  
- **Clustering**: Identifying communities in social or biological networks.

---

### 2. Weighted vs. Unweighted Graphs

#### **What are Edge Weights?**
Weights add additional data (e.g., cost, distance, or capacity) to edges, enhancing graph applications.

#### **Weighted Graphs**

**Definition**  
A weighted graph has edges with associated weights or costs.

**Key Properties**  
- Edges are represented as `(u, v, w)`, where `w` is the weight.  
- Weights can be positive or negative but are typically non-negative.

**Examples**  
- **Transportation Networks**: Roads connecting cities, with weights representing distances or travel times.  
- **Telecommunication Networks**: Connections between routers, with weights for latency or bandwidth.

**Use Cases**  
- **Shortest Path Algorithms**:  
  - *Dijkstra's Algorithm*: Finds shortest paths in graphs with non-negative weights.  
  - *Bellman-Ford Algorithm*: Handles graphs with negative weights.  
- **Minimum Spanning Trees**:  
  - Algorithms like *Kruskal's* or *Prim's* minimize the total weight.

---

#### **Unweighted Graphs**

**Definition**  
An unweighted graph treats all edges equally, with no associated costs.

**Key Properties**  
- Edges are represented as `(u, v)` without weights.  
- Connections are binary (exist or not).

**Examples**  
- **Social Networks**: Represent simple friend/follower connections.  
- **Connectivity Testing**: Determine whether nodes are reachable.

**Use Cases**  
- **Breadth-First Search (BFS)**: Find the shortest path by counting edges.  
- **Depth-First Search (DFS)**: Explore connectivity or detect cycles.

---

### Comparison Table

| Feature              | Directed Graph          | Undirected Graph       |
|----------------------|-------------------------|------------------------|
| **Edge Representation** | Ordered Pair `(u, v)`  | Unordered Pair `{u, v}`|
| **Edge Direction**     | One-way                | Two-way                |
| **Use Cases**          | Task scheduling, data flow | Social networks, clustering |

| Feature              | Weighted Graph          | Unweighted Graph       |
|----------------------|-------------------------|------------------------|
| **Edge Representation** | `(u, v, w)` (weight `w`) | `(u, v)` (no weight)   |
| **Additional Data**    | Yes (weights/costs)     | No                     |
| **Use Cases**          | Transportation, optimization | Simple connectivity    |

---

## Dynamic Programming

Dynamic Programming (DP) is a powerful optimization technique used to solve problems by breaking them into smaller overlapping subproblems. Solutions to these subproblems are stored to avoid redundant computations.

### Key Concepts of DP

1. **Optimal Substructure**  
   - A problem has optimal substructure if its solution can be derived from solutions to smaller subproblems.

2. **Overlapping Subproblems**  
   - A problem exhibits overlapping subproblems when the same computations are repeated multiple times.

---

### Steps to Solve a DP Problem

1. **Define the State**  
   - Represent subproblems using a `dp` array or table.

2. **State Transition**  
   - Establish relationships between current and previous states.

3. **Base Case**  
   - Define the simplest problem scenario to start computations.

4. **Compute and Optimize**  
   - Use bottom-up iteration or recursion with memoization.

---

### Applications of DP

- **Fibonacci Numbers**:  
  `dp[i] = dp[i-1] + dp[i-2]`

- **Knapsack Problem**:  
  Maximize value within weight constraints.

- **Longest Common Subsequence**:  
  Identify the longest subsequence shared by two sequences.

- **Graph Shortest Paths**:  
  Algorithms like *Floyd-Warshall* use DP to find shortest paths between all pairs of vertices.



