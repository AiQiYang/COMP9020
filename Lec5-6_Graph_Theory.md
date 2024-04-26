# Terminology and Notation

## Graph

A graph is represented by a pair (V, E) where:
- V: set of vertices
- E: set of edges

## Undirected Graph

Every edge e ∈ E is a two-element set of vertices, i.e., e = {x, y} ⊆ V where x ≠ y

## Directed Graph

Every edge (or arc) e ∈ E is an ordered pair of vertices, i.e., e = (x, y) ∈ V × V, where x may equal y.

## Graph Representation

1. **Pictorially**
2. **Adjacency matrix**

![Adjacency Matrix]()

1. **Incidence matrix**
   - Each row represents a vertex
   - Each column represents an edge

![Incidence Matrix]()

## Path

- **(Directed) walk:** a sequence of edges
- **Trail:** a walk where **no edge is repeated**
- **Path:** a walk where **no vertex is repeated**
- **Length of a walk:** the number of edges, may contain duplicate vertices and/or edges
- **Subpath / Subwalk:** a portion of a path from one vertex to another in a graph

## Connectedness

- **Connected set/graph (undirected):** Every pair of vertices is connected by a path.
- **Strongly connected set/graph (directed):** Every pair of vertices is connected by a bidirectional directed path.
- **Connected Component:** A set of vertices where every pair of vertices can be connected by a path, and the set is maximal (no additional vertices can be added without breaking the property).

## Vertex Degree (Undirected graphs)

- **Degree of a vertex:** The number of edges connected to it.
- **Regular graph:** If every vertex in the graph has the same degree.
- **Degree sequence:** $D_0, D_1, D_2, . . . , D_k$ of graph $G = (V , E)$, where $D_i$ is the number of vertices of degree $i$.

### Fact:

- $\sum_{v \in V} \text{deg}(v) = 2 \cdot |E|$
    - The sum of vertex degrees is always even.
    - There is an even number of vertices of odd degree.

## Vertex Degree (Directed graphs)

- **Out-degree of a vertex:** The number of edges going out of the vertex.
- **In-degree of a vertex:** The number of edges going into the vertex.

### Fact:

$\sum_{v \in V} \text{outdeg}(v) = \sum_{v \in V} \text{indeg}(v) = |E|$

## Cycles

- **Closed walk:** A walk where the starting and ending vertices are the same.
- **Cycle:** A closed path in the graph where all vertices, except the start and end, are distinct.
    - 3 or more in undirected graph
    - 2 or more in directed graphs
- **Acyclic walk:** A walk where no vertex is repeated.

**The definition of a cycle:**

A cycle is defined such that removing any single edge from it leaves a path.

**Sufficient condition for a cycle:**

A cycle C = (v1, v2, ..., vn) is a cycle if removing any single edge leaves a path.

## Tree

- **Connected** **acyclic** [**undirected**] graph
- **Forest:** A set of disjoint trees

**Graph G is a tree iff:**

1. It is acyclic, and the number of vertices equals the number of edges plus one.
2. There is exactly one path between any two vertices.
3. G is connected, but becomes disconnected if any single edge is removed.
4. G is acyclic, but adding any single edge between existing vertices forms a cycle.

## Bipartite Graphs

- Vertices can be divided into **two disjoint sets**.
- Each edge must connect a vertex from one set to a vertex from the other set.

## Special Graphs

- **Complete Graph:**
    - n vertices, all pairwise connected, $\frac{n(n - 1)}{2}$ edges
- **Complete bipartite graph** $K_{m,n}$
    - Has m + n vertices, partitioned into two disjoint sets, one of n, the other of m vertices.
    - All vertices from different parts are connected; vertices from the same part are disconnected. No. of edges is m · n.
- **Complete k-partite graph** $K_{m1,...,mk}$
    - Has m1 + . . . +
