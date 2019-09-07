# Implementation-of-a-Graph

1. Implementation of a Graph as an Adjacency List

    (1) Using dictionaries, it is easy to implement the adjacency list in Python. In our implementation of the Graph abstract data type we 
    will create two classes: Graph, which holds the master list of vertices, and Vertex, which will represent each vertex in the graph.

    (2) Each Vertex uses a dictionary to keep track of the vertices to which it is connected, and the weight of each edge. This dictionary     is called connectedTo. The constructor simply initializes the id, which will typically be a string, and the connectedTo dictionary. The 
    addNeighbor method is used add a connection from this vertex to another. The getConnections method returns all of the vertices in the 
    adjacency list, as represented by the connectedTo instance variable. The getWeight method returns the weight of the edge from this         vertex to the vertex passed as a parameter.
  
    (3) In order to implement a Graph as an Adjacency List what we need to do is define the methods our Adjacency List object will have:

        (i) Graph() creates a new, empty graph.
        (ii) addVertex(vert) adds an instance of Vertex to the graph.
        (iii) addEdge(fromVert, toVert) Adds a new, directed edge to the graph that connects two vertices.
        (iv) addEdge(fromVert, toVert, weight) Adds a new, weighted, directed edge to the graph that connects two vertices.
        (v) getVertex(vertKey) finds the vertex in the graph named vertKey.
        (vi) getVertices() returns the list of all vertices in the graph.
        (vii) in returns True for a statement of the form vertex in graph, if the given vertex is in the graph, False otherwise.

2. Implementation of Graph with OrderedDict

    Implement a simple graph by focusing on the Node class. The graph will be directed and the edges can hold weights. We will have three       classes, a State class, a Node class, and finally the Graph class.We're going to be taking advantage of two built-in tools here,           OrderDict and Enum.
