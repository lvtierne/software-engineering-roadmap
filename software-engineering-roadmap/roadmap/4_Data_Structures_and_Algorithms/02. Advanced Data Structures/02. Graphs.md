# Graphs

Graphs are data structures used to represent networks of nodes and edges.

## Key Concepts
- **Nodes (Vertices)**: Entities or points in a graph.
- **Edges**: Connections between nodes.
- **Types**: Directed vs. undirected, weighted vs. unweighted, cyclic vs. acyclic.

## Example: Python Graph Implementation
```python
class Graph:
    def __init__(self):
        self.graph = {}

    def add_vertex(self, vertex):
        if vertex not in self.graph:
            self.graph[vertex] = []

    def add_edge(self, vertex1, vertex2):
        if vertex1 in self.graph and vertex2 in self.graph:
            self.graph[vertex1].append(vertex2)
            self.graph[vertex2].append(vertex1)

    def display(self):
        for vertex in self.graph:
            print(f"{vertex}: {self.graph[vertex]}")
```

## Learning Resources

- [Graph Data Structures - GeeksforGeeks](https://www.geeksforgeeks.org/graph-data-structure-and-algorithms/)
- [Graphs in Python - Tutorialspoint](https://www.tutorialspoint.com/python_data_structure/python_graphs.htm)

## Next Steps

1. Implement graph traversal algorithms like BFS and DFS.
2. Solve problems related to graph theory and algorithms.
