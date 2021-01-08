[Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
Edge - An edge is a connection between two nodes.
Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
Degree - The degree of a vertex is the number of edges connected to that vertex.

there are undirected and directed graphs.

An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

A Directed Graph also called a Digraph is a graph where every edge is directed.

Complete Graphs are graphs when all nodes are connected to eachother.

connected graphs are graphs where each node has at least one edge.

a disconnected (the most cooked) graph is a graph where some nodes dont have edges(are not connected to other nodes)

Acyclic Graph
An acyclic graph is a directed graph without cycles.

all nodes point to other nodes and never back to themselves.

Cyclic Graphs
A Cyclic graph is a graph that has cycles.

the nodes create a circle, node one points at two, two points at three, and three points at one. Or one points at two, and two  points at one.

Adjacency Matrix
An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

Weighted Graphs
A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights. This is what a weighted graph looks like:

You can do breadth first traversals on these graphs which utilizes queues.

You can do depth first traversal on these graphs which uses a stack.


Real World Uses of Graphs
Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

GPS and Mapping
Driving Directions
Social Networks
Airline Traffic
Netflix uses graphs for suggestions of products

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)