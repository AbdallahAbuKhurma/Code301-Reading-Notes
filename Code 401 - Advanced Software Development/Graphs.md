# Graphs
>
**A graph** is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

* Here is some common terminology used when working with Graphs:

  * Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
  
  * Edge - An edge is a connection between two nodes.
  
  * Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
  
  * Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

* Undirected Graphs

        An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

* Directed Graphs (Digraph)

        A Directed Graph also called a Digraph is a graph where every edge is directed. Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

## Complete vs Connected vs Disconnected

* A complete graph is when all nodes are connected to all other nodes.

* A connected graph is graph that has all of vertices/nodes have at least one edge.

* A disconnected graph is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

* Acyclic: directed graph without cycles

* Cycle: when a node can be traversed through and potentially end up back at itself

* Directed acyclic graph (DAG): can also be represented as what we know as a tree

* Cyclic: graph that has cycles

* Cycle: defined as a path of a positive length that starts and ends at the same vertex

## Weighted Graphs

**Weighted graph:** graph with numbers assigned to its edges, the numbers are called weights
When representing a weighted graph in a matrix, you set the element in the 2D array to represent the actual weight between the two paths

## Traversals

1. Breadth First: In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. The breadth-first traversal of a graph is like that of a tree, with the exception that graphs can have cycles

2. Depth First: In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. Similar to how the breadth-first uses a queue, we are going to use a Stack for our depth-first traversal.

## Resources

[Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)
