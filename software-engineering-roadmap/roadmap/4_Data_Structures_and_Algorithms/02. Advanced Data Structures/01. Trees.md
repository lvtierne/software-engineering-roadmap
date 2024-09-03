# Trees

A tree is a hierarchical data structure consisting of nodes, where each node has zero or more child nodes.

## Key Concepts
- **Nodes**: Basic units of a tree, including the root, internal nodes, and leaves.
- **Binary Trees**: Each node has at most two children (left and right).
- **Binary Search Trees (BST)**: A binary tree where each node's left subtree has smaller values and the right subtree has larger values.

## Example: Python Binary Tree Implementation
```python
class TreeNode:
    def __init__(self, key):
        self.left = None
        self.right = None
        self.value = key

class BinaryTree:
    def __init__(self):
        self.root = None

    def insert(self, key):
        if self.root is None:
            self.root = TreeNode(key)
        else:
            self._insert(self.root, key)

    def _insert(self, root, key):
        if key < root.value:
            if root.left is None:
                root.left = TreeNode(key)
            else:
                self._insert(root.left, key)
        else:
            if root.right is None:
                root.right = TreeNode(key)
            else:
                self._insert(root.right, key)

    def inorder_traversal(self, root):
        if root:
            self.inorder_traversal(root.left)
            print(root.value, end=' ')
            self.inorder_traversal(root.right)
```

## Learning Resources

- [Tree Data Structures - GeeksforGeeks](https://www.geeksforgeeks.org/tree-data-structure/)
- [Binary Trees - Tutorialspoint](https://www.tutorialspoint.com/data_structures_algorithms/tree_data_structure.htm)

## Next Steps

1. Implement various tree traversal algorithms.
2. Solve problems related to tree operations and properties.
