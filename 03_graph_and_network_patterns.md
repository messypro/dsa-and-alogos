# Playbook 03: Graph & Network Topology Patterns

Detailed progression maps and targeting matrices for linked topologies, matrices, dependencies, and network structures.

## Category C: Graph & Network Topology

### 8. Breadth-First Search (BFS)
*   **The Core Concept:** Level-by-level neighborhood traversal using a queue structure to guarantee structural layer properties.
*   **Trigger Keywords:** "Shortest path in unweighted graph", "Minimum steps to convert X to Y", "Level-order traversal", "Nearest neighbor grid mapping".
*   **Staff-Level Reality:** Standard baseline pattern for modeling service networks, cluster node communication hops, or asset routing pipelines.
*   **Progression Mechanics:**
    *   *Easy:* Basic binary tree level-by-level sweep.
    *   *Medium:* Tracking shortest paths over multi-directional 2D grid spaces while maintaining visited maps to prevent loops.
    *   *Hard:* Modifying node state layers dynamically (0-1 BFS or Dijkstra-adjacent transformations) where step cost depends on the path taken.
*   **High-Yield LeetCode Targets:**
    *   *Easy:* 102. Binary Tree Level Order Traversal
    *   *Medium:* 994. Rotting Oranges
    *   *Hard:* 126. Word Ladder II

### 9. Depth-First Search (DFS)
*   **The Core Concept:** Exhaustively diving down a single network or structural branch before winding back up, utilizing a runtime execution stack.
*   **Trigger Keywords:** "Find any path", "Connected components", "Clone graph", "Tree serialization", "Graph cycle detection".
*   **Staff-Level Reality:** Applied to recursive entity models, directory tree indexing, parsing Abstract Syntax Trees (ASTs), or resolving deep object maps.
*   **Progression Mechanics:**
    *   *Easy:* Simple tree traversal tasks like counting nodes or identifying maximum depth limits.
    *   *Medium:* Traversing cross-linked cyclic object networks or isolated grid sectors, requiring explicit cycle protection.
    *   *Hard:* Tracking multiple paths and long-term state across very deep graph topologies where you must use manual stack implementations to prevent stack overflow.
*   **High-Yield LeetCode Targets:**
    *   *Easy:* 104. Maximum Depth of Binary Tree
    *   *Medium:* 200. Number of Islands
    *   *Hard:* 329. Longest Increasing Path in a Matrix

### 10. Topological Sort
*   **The Core Concept:** Creating a linear execution pathway from a Directed Acyclic Graph (DAG) based on strict directionality rules.
*   **Trigger Keywords:** "Prerequisites", "Build order", "Task scheduling", "Dependency resolution matrix".
*   **Staff-Level Reality:** Mimics real-world continuous deployment (CI/CD) pipelines, package managers (npm/pip dependency calculation), or task orchestration graphs (Airflow).
*   **Progression Mechanics:**
    *   *Easy:* Straight dependency lists with guaranteed legal validation states.
    *   *Medium:* Utilizing Kahn's algorithm or DFS state colors to process scheduling orders while cleanly identifying illegal processing loops (cycles).
    *   *Hard:* Multi-layered scheduling requests where processing jobs have custom costs or deadlines, requiring you to mix priorities into the execution stream.
*   **High-Yield LeetCode Targets:**
    *   *Easy:* 1716. Calculate Money in Leetcode Bank (Simple series progression analogy)
    *   *Medium:* 207. Course Schedule
    *   *Hard:* 269. Alien Dictionary

### 11. Union-Find (Disjoint Set Union - DSU)
*   **The Core Concept:** Storing and grouping partitioned elements into disjoint subsets to quickly answer whether two objects are part of the same island or network cluster.
*   **Trigger Keywords:** "Connected components", "Network connectivity", "Redundant connections", "Dynamic graph partitioning", "Accounts merge".
*   **Staff-Level Reality:** Evaluates cluster segmentation, network isolation problems, or live user group clustering algorithms.
*   **Progression Mechanics:**
    *   *Easy:* Direct connection lists parsed sequentially without tracking rankings or optimizations.
    *   *Medium:* Standard implementation built cleanly with path compression and union-by-rank to isolate loops or merge complex record sets.
    *   *Hard:* Real-time grid mutations where connections change over time, requiring you to track structural attributes dynamically or unwind previous operations.
*   **High-Yield LeetCode Targets:**
    *   *Easy:* 1971. Find if Path Exists in Graph
    *   *Medium:* 547. Number of Provinces
    *   *Hard:* 305. Number of Islands II
