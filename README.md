# 🌳 Binary Search Tree — Python

A clean, object-oriented implementation of a Binary Search Tree (BST) in Python supporting insertion, search, deletion, and in-order traversal.

## 📌 What is a BST?

A Binary Search Tree is a hierarchical data structure where:
- **Left child** is always smaller than the parent
- **Right child** is always greater than the parent
- This property makes **search extremely efficient — O(log n)**

## ⚙️ Features

- ✅ Insert nodes
- ✅ Search for a value
- ✅ Delete nodes (handles all 3 cases)
- ✅ In-order traversal (returns sorted output)
- ✅ No external libraries required

## 🗂️ Project Structure
```
bst.py        — Main implementation (TreeNode + BinarySearchTree classes)
```

## 🚀 Usage
```python
bst = BinarySearchTree()
nodes = [50, 30, 20, 40, 70, 60, 80]

for node in nodes:
    bst.insert(node)

print('Search for 80:', bst.search(80))
print('Inorder traversal:', bst.inorder_traversal())

bst.delete(40)

print('Search for 40:', bst.search(40))
print('Inorder traversal after deleting 40:', bst.inorder_traversal())
```

## 📤 Output
```
Search for 80: 80
Inorder traversal: [20, 30, 40, 50, 60, 70, 80]
Search for 40: None
Inorder traversal after deleting 40: [20, 30, 50, 60, 70, 80]
```

## 🧠 Deletion — 3 Cases Handled

| Case | Description |
|------|-------------|
| Leaf Node | Simply removed |
| One Child | Replaced by its child |
| Two Children | Replaced by in-order successor |

## 📌 Concepts Demonstrated

- Object-Oriented Programming (OOP)
- Recursive Algorithms
- Binary Search Tree Properties
- In-Order Traversal
- Edge Case Handling

## ⚙️ Requirements

- Python 3.x
- No external libraries needed
