# Graphs

A graph is a non-linear data strcuture that can be looked at as a collection of `verticies` (or `nodes`) potentially connected by line segments named `edges`

Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
Edge - An edge is a connection between two nodes.
Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
Degree - The degree of a vertex is the number of edges connected to that vertex.


### Undirected Graphs

An `Unidirectde Graph` is a graph where each edge is unidrected or bi-directional. This means that the undirected graph does not move in any direction

For example, in the graph below, Node `C` is connected to `Node A`, `Node E` and `Node B`. There are no "directions" given to point to specific verticies. The connection is bi-directional

A `Directed Graph` also called a `Digraph` is a graph where every page is directed


### Complete Graphs 

A complete graph is when all nodes are connected to all other nodes

### Connected Graph

A conencted graph is a graph that has all of `verticies`/`nodes` have at least one edge

### Disconnected

A disconnected graph is a graph where some verticies may not have edges

### Acyclic Graph

A acyclic graph is a directed graph without cycles

### Cyclic Graphs

A Cyclic graph is a graph that has cycles

### Adjacency Matric

An adjacency matric is represented through a 2-dimensional array. If there n verticies, then we are looking at an n x n Boolean matrix. 

### Adjacency List

An adjacency list ist he most common way to represent graphs

### Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights. This is what a weighted graph loosk like:

### Breadth first traversal
  
  
  
    ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    DECLARE visited <-- new Set()

    breadth.Enqueue(vertex)
    visited.Add(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                visited.Add(child)
                breadth.Enqueue(child)

    return nodes;

### Depth First 

`Push` the root node into the Stack and mark as visited.

Start a while loop that runs as long as the stack is not empty.

`Pop` the top node off of the stack and check its neighbors.

If a neighbor hasn’t been visited, push it onto the stack and mark as visited.
Repeat until the stack is empty.
