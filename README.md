# ⚫ Graph Theory in Tech Interviews 2024: 17 Must-Know Questions & Answers

**Graph Theory** deals with networks of interconnected nodes and edges. It provides the foundation for understanding structures and pathways in various applications, from social networks to transportation systems. In coding interviews, it is used to assess a candidate's understanding of **graph traversal**, **pathfinding**, and **network analysis** techniques.

Check out our carefully selected list of **basic** and **advanced** Graph Theory questions and answers to be well-prepared for your tech interviews in 2024.

![Graph Theory Decorative Image](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/blogImg%2FgraphTheory.png?alt=media&token=c8cc625e-9d11-40e2-85b6-72014a67744a&_gl=1*13wtkkg*_ga*OTYzMjY5NTkwLjE2ODg4NDM4Njg.*_ga_CW55HF8NVT*MTY5ODYwNTk1NS4xOTAuMS4xNjk4NjA3MjUzLjIzLjAuMA..)

👉🏼 You can also find all answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 1. What is a _Graph_?

### Answer

A **graph** is a data structure that represents a collection of interconnected **nodes** through a set of **edges**.

This abstract structure is highly versatile and finds applications in various domains, from social network analysis to computer networking.

### Core Components

A graph consists of two main components:

1. **Nodes**: Also called **vertices**, these are the fundamental units that hold data.
2. **Edges**: These are the connections between nodes, and they can be either **directed** or **undirected**.

### Visual Representation

![Graph: Unidirected, Directed, Cyclic, Acyclic, Weighted, Unweighted, Sparse, Dense](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fwhat-is-graph.png?alt=media&token=0d7b76b3-23d6-4a72-99d8-1b84565274b4)

### Graph Representations

There are several ways to represent graphs in computer memory, with the most common ones being **adjacency matrix**, **adjacency list**, and **edge list**.

#### Adjacency Matrix

In an adjacency matrix, a 2D Boolean array indicates the edges between nodes. A value of `True` at index `[i][j]` means that an edge exists between nodes `i` and `j`.

Here is the Python code:

```python
graph = [
    [False, True, True],
    [True, False, True],
    [True, True, False]
]
```

#### Adjacency List

An adjacency list represents each node as a list, and the indices of the list are the nodes. Each node's list contains the nodes that it is directly connected to.

Here is the Python code:

```python
graph = {
    0: [1, 2],
    1: [0, 2],
    2: [0, 1]
}
```

#### Edge List

An edge list is a simple list of tuples, where each tuple represents an edge between two nodes.

Here is the Python code:

```python
graph = [(0, 1), (0, 2), (1, 2)]
```

---

## 🔹 2. What are some common _Types_ and _Categories_ of _Graphs_?

### Answer

Graphs serve as **adaptable data structures** for various computational tasks and real-world applications. Let's look at their diverse types.

### Types of Graphs

1. **Undirected**: Edges lack direction, allowing free traversal between connected nodes. Mathematically, $(u,v)$ as an edge implies $(v,u)$ as well.
2. **Directed (Digraph)**: Edges have a set direction, restricting traversal accordingly. An edge $(u,v)$ doesn't guarantee $(v,u)$.

![Graph Types: Unidirected, Directed](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fdirection.png?alt=media&token=187d88ba-04f3-4993-bbcf-f3bc35c41c0d)

#### Weight Considerations

1. **Weighted**: Each edge has a numerical "weight" or "cost."
2. **Unweighted**: All edges are equal in weight, typically considered as 1.

![Graph Types: Weighted, Unweighted](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fweight.png?alt=media&token=c975e0b9-4c21-4518-8c7e-9489279b642b)

#### Presence of Cycles

1. **Cyclic**: Contains at least one cycle or closed path.
2. **Acyclic**: Lacks cycles entirely.

![Graph Types: Cyclic, Acyclic](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fcyclic.png?alt=media&token=f072557c-d298-4c73-b5b8-11ca014eeb08)

#### Edge Density

1. **Dense**: High edge-to-vertex ratio, nearing the maximum possible connections.
2. **Sparse**: Low edge-to-vertex ratio, closer to the minimum.

![Graph Types: Sparse, Dense](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fdensity.png?alt=media&token=084eec75-b348-4429-ae30-788ac7f49778)

#### Connectivity

1. **Connected**: Every vertex is reachable from any other vertex.
2. **Disconnected**: Some vertices are unreachable from others.

![Graph Types: Connected, Disconnected](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fconnected-disconnected-graph.png?alt=media&token=3aa6db3e-852e-4c62-a42d-a6ebf501d9f7)

#### Edge Uniqueness

1. **Multigraph**: Allows duplicate edges between vertices.
2. **Simple**: Limits vertices to a single connecting edge.

![Graph Types: Multigraph, Simple Graph](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Fsimple-multigraph.png?alt=media&token=a7c888e1-a317-470c-94b8-bf998880bdd7)

---

## 🔹 3. What are some real-world _Applications_ of _Graphs_?

### Answer

**Graphs** are foundational to numerous domains, **directly or indirectly** influencing our daily activities. Whether you're navigating online, problem-solving, or gaming, chances are you're benefiting from graph-based systems and algorithms.

### Practical Applications

1. **Computer Networks**: Graphs model the connections between routers and servers.
  
2. **Core Data Structures**: Trees and linked lists are special types of graphs.
  
3. **Routing Algorithms**: Essential for GPS and mapping services like Google Maps.

4. **Constraint Resolution**: Useful in scheduling and optimization tasks, such as university course scheduling.

5. **Chemical Modeling**: Represents molecular structures for better understanding of chemical interactions.

6. **Project Management**: Aids in activity scheduling and resource allocation.

7. **Code Parsing**: Abstract Syntax Trees (ASTs) in compilers are specific kinds of directed acyclic graphs (DAGs).

8. **State Control**: State machines govern various systems, from network protocols to video games.

9. **Machine Learning Pipelines**: Involved in data preprocessing and relationship modeling.

10. **Text Recognition**: Vital in optical character recognition algorithms.

11. **Decision-making Algorithms**: Employed in logistics, finance, and more for optimal choices.

### Graphs in Modern Tech

The influence of **graph theory** extends to several cutting-edge technologies:

- **Web Search**: Graphs help optimize and analyze the structure of the internet for search engines.

- **Social Media**: Platforms like Facebook function fundamentally as expansive graphs.

- **User Recommendations**: Algorithms for suggestions often use graphs to model user behavior.

- **Financial Risk Assessment**: Used in banking for activities like fraud detection and risk evaluation.

---

## 🔹 4. Compare _Adjacency Lists_ and _Adjacency Matrices_ for graph representation.

### Answer

Graphs can be represented in various ways, but **Adjacency Matrix** and **Adjacency List** are the most commonly used data structures. Each method offers distinct advantages and trade-offs, which we'll explore below.

![Example Graph](https://static.javatpoint.com/tutorial/graph-theory/images/graph-representations1.png)

### Space Complexity

- **Adjacency Matrix**: Requires a $N \times N$ matrix, resulting in $O(N^2)$ space complexity.
- **Adjacency List**: Utilizes a list or array for each node's neighbors, leading to $O(N + E)$ space complexity, where $E$ is the number of edges.

### Time Complexity for Edge Look-Up

- **Adjacency Matrix**: Constant time, $O(1)$, as the presence of an edge is directly accessible.
- **Adjacency List**: Up to $O(k)$, where $k$ is the degree of the vertex, as the list of neighbors may need to be traversed.

### Time Complexity for Traversal

- **Adjacency Matrix**: Requires $O(N^2)$ time to iterate through all potential edges.
- **Adjacency List**: Takes $O(N + E)$ time, often faster for sparse graphs.

### Time Complexity for Edge Manipulation

- **Adjacency Matrix**: $O(1)$ for both addition and removal, as it involves updating a single cell.
- **Adjacency List**: $O(k)$ for addition or removal, where $k$ is the degree of the vertex involved.

### Time Complexity for Vertex Manipulation

- **Adjacency Matrix**: $O(N^2)$ as resizing the matrix is needed.
- **Adjacency List**: $O(1)$ as it involves updating a list or array.

### Code Example: Adjacency Matrix & Adjacency List

Here is the Python code:

```python
adj_matrix = [
    [0, 1, 1, 0, 0, 0],
    [1, 0, 0, 1, 0, 0],
    [1, 0, 0, 0, 0, 1],
    [0, 1, 0, 0, 1, 1],
    [0, 0, 0, 1, 0, 0],
    [0, 0, 1, 1, 0, 0]
]

adj_list = [
    [1, 2],
    [0, 3],
    [0, 5],
    [1, 4, 5],
    [3],
    [2, 3]
]
```

---

## 🔹 5. What is the difference between a _Tree_ and a _Graph_?

### Answer

**Graphs** and **trees** are both nonlinear data structures, but there are fundamental distinctions between them.

### Key Distinctions

- **Uniqueness**: Trees have a single root, while graphs may not have such a concept.
- **Topology**: Trees are **hierarchical**, while graphs can exhibit various structures.
-  **Focus**: Graphs center on relationships between individual nodes, whereas trees emphasize the relationship between nodes and a common root.

### Graphs: Versatile and Unstructured

- **Elements**: Composed of vertices/nodes (denoted as V) and edges (E) representing relationships. Multiple edges and **loops** are possible.
- **Directionality**: Edges can be directed or undirected.
- **Connectivity**: May be **disconnected**, with sets of vertices that aren't reachable from others.
- **Loops**: Can contain cycles.

### Trees: Hierarchical and Organized

- **Elements**: Consist of nodes with parent-child relationships.
- **Directionality**: Edges are strictly parent-to-child.
- **Connectivity**: Every node is accessible from the unique root node.
- **Loops**: Cycles are not allowed.

### Visual Representation

![Graph vs Tree](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/graph-theory%2Ftree-graph.jpg?alt=media&token=0362c5d3-e851-4cd2-bbb4-c632e77ccede&_gl=1*euedhq*_ga*OTYzMjY5NTkwLjE2ODg4NDM4Njg.*_ga_CW55HF8NVT*MTY5NzI4NzY1Ny4xNTUuMS4xNjk3Mjg5NjU2LjYwLjAuMA..)

---
## 🔹 6. Explain the _Breadth-First Search_ (BFS) traversing method.

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 7. Explain the _Depth-First Search_ (DFS) algorithm.

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 8. Why the complexity of _DFS_ is _O(V+E)_?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 9. What are the key differences between _BFS_ and _DFS_?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 10. Why does _Breadth-First Search_ use more memory than _Depth-First Search_?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 11. Illustrate the difference in _Peak Memory Consumption_ between _DFS_ and _BFS_.

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 12. Provide some practical examples of using _Depth-First Search_ vs _Breadth-First Search_.

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 13. What is difference between _BFS_ and _Dijkstra's_ algorithms when looking for shortest path?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 14. What is _A\* Search_?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 15. What is heuristic cost function in _A\* Search_?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 16. Explain the difference between _Best-First Search_ and _A\* Search_.

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

## 🔹 17. What is _Bipartite Graph_? How to detect one?

### Answer

👉🏼 Check out all 17 answers here: [Devinterview.io - Graph Theory](https://devinterview.io/data/graphTheory-interview-questions)

---

