# Class 15

## Trees

**Common Terminology**

Node - A Tree node is a component which may contain its own values, and references to other nodes

Root - The root is the node at the beginning of the tree

K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

Left - A reference to one child node, in a binary tree

Right - A reference to the other child node, in a binary tree

Edge - The edge in a tree is the link between a parent and child node

Leaf - A leaf is a node that does not have any children

Height - The height of a tree is the number of edges from the root to the furthest leaf

![binaryTree](assets/BinaryTree1.png)

**Tree traversals**

The two categories of traversing trees is Depth first and Breadth first.

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

Pre-order: root >> left >> right

In-order: left >> root >> right

Post-order: left >> right >> root

Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree.


references

[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)


<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)