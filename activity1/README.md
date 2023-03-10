# Activities

## Task 1: Tree Definition

- Answer at least 5 questions from the following link. Make sure you write the question as well as the answer.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Binary/DefSumm.html

1. What is the minimum number of internal nodes in a binary tree with 8 nodes?
//4

2. Which statement is false?

[]Every non-root node in a binary tree has exactly one parent
[]Every non-empty binary tree has exactly one root node
[x]Every binary tree has at least one node
[] node in a binary tree has exactly two children
[]None of the above

3. What is the minimum number of nodes in a full binary tree with height 3?
//7

4. Suppose T is a binary tree with 14 nodes. What is the minimum possible height of T?
//3

5. Which statement is false?

[x]Every binary tree has at least one node
[]Every non-empty binary tree has exactly one root node
[]Every non-root node in a binary tree has exactly one parent
[]Every node in a binary tree has exactly two children
[]None of the above



## Task 2

- Explain how the code in ./src/bt.cpp works. Refer to the following link:
  https://www.geeksforgeeks.org/binary-tree-array-implementation/

The given code is an implementation of a binary tree using an array. In this implementation, the tree is represented as an array of characters, where each node of the tree is a character in the array.

The functions in the code are as follows:

1. root(char key) - This function is used to set the root of the tree. It takes a character key as an argument, which is the value of the root node. If the root of the tree is already set, it prints a message saying "Tree already had root", otherwise, it sets the root node to the given value and returns 0.

2. set_left(char key, int parent) - This function is used to set the left child of a node in the tree. It takes two arguments - a character key which is the value of the left child node, and an integer parent which is the index of the parent node in the array. If the parent node is not found in the array (i.e. its value is '\0'), it prints a message saying "Can't set child", otherwise, it sets the left child node of the parent node to the given value and returns 0.

3. set_right(char key, int parent) - This function is used to set the right child of a node in the tree. It takes two arguments - a character key which is the value of the right child node, and an integer parent which is the index of the parent node in the array. If the parent node is not found in the array (i.e. its value is '\0'), it prints a message saying "Can't set child", otherwise, it sets the right child node of the parent node to the given value and returns 0.

4. print_tree() - This function is used to print the entire tree. It loops through the array and prints each character in the array, representing a node of the tree. If the value of the node is '\0', it prints a dash '-' instead.

The main() function is used to create a sample binary tree using the functions defined above. It sets the root node to 'A', sets its left child to 'B' and its right child to 'C'. It then sets the left child of 'B' to 'D', its right child to 'E', and the right child of 'C' to 'F'. Finally, it prints the entire tree using the print_tree() function.

## Task 3: Tree Traversal

Refer to te following links. Discuss the difference between the different ways binary trees can be traversed.

- [Pre-order Traversal](https://opendsa-server.cs.vt.edu/OpenDSA/AV/Binary/btTravPreorderPRO.html)
- [Post-order Traversal](https://opendsa-server.cs.vt.edu/OpenDSA/AV/Binary/btTravPostorderPRO.html)
- [In-order Traversal](https://opendsa-server.cs.vt.edu/OpenDSA/AV/Binary/btTravInorderPRO.html)


1. Pre-order Traversal - In pre-order traversal, we visit the root node first, followed by the left subtree, and then the right subtree. This traversal follows the "node, left, right" order. Pre-order traversal is useful when we want to create a copy of the tree, or when we want to print the prefix expression of an expression tree.

2. In-order Traversal - In in-order traversal, we visit the left subtree first, followed by the root node, and then the right subtree. This traversal follows the "left, node, right" order. In-order traversal is useful when we want to print the infix expression of an expression tree, or when we want to visit the nodes of the tree in sorted order.

3. Post-order Traversal - In post-order traversal, we visit the left subtree first, followed by the right subtree, and then the root node. This traversal follows the "left, right, node" order. Post-order traversal is useful when we want to delete the entire tree, or when we want to print the postfix expression of an expression tree.

In summary, the difference between the different ways of traversing a binary tree is the order in which the nodes are visited. The order of traversal affects the way we can process the nodes and can be chosen based on the requirements of the problem at hand.

## Task 4: Individual (at home)

- Answer at least 5 questions from the following link. Make sure you write the question as well as the answer.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Binary/TravSumm.html

1. If you are given the order of the nodes as visited by a postorder traversal and the order of the nodes as visited by an inorder traversal, do you have enough information to reconstruct the original tree? Assume that the nodes all have unique values.
// True
2. If you are given the order of the nodes as visited by a preorder traversal and the order of the nodes as visited by an inorder traversal, do you have enough information to reconstruct the original tree? Assume that the nodes all have unique values.
//True
3. Visiting each element in a tree is known as:

[]Merging
[]Inserting
[]Sorting
[x]Traversing
[]Enumerating
4. If you are given the order of the nodes as visited by a preorder traversal and the order of the nodes as visited by a postorder traversal, do you have enough information to reconstruct the original tree? Assume that the nodes all have unique values.
//False
5. If you are given the order of the nodes as visited by a preorder traversal and the order of the nodes as visited by an inorder traversal, do you have enough information to reconstruct the original tree? Assume that the nodes all have unique values.
//True

- Answer at least 5 questions from the following link. Make sure you write the question as well as the answer.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Binary/Treeprobs.html

  

## Links

- https://cpp.sh/
- https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/BinaryTree.html
- https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/BinaryTreeTraversal.html
