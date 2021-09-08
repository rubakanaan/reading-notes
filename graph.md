# Graphs


* A **graph** is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

### Terminology used when working with Graphs:

1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. Edge - An edge is a connection between two nodes.
2. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
3. Degree - The degree of a vertex is the number of edges connected to that vertex.


### Directed vs Undirected

1. Undirected Graphs
    * An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

2. Directed Graphs (Digraph)
    * A Directed Graph also called a Digraph is a graph where every edge is directed.

    * Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.


### Graph Representation
We represent graphs through:

1. Adjacency Matrix
    * An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix
    * Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.
2. Adjacency List
    * An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

    * Adjacency lists make it easy to view if one vertices connects to another.

### Traversals

1. Breadth First
2. Depth First

