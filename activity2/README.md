# Activities

## Task 1

- Refer to the following link. Discuss how Binary Search Trees work:
  https://www.cs.usfca.edu/~galles/visualization/BST.html

  //Binary Search Trees (BSTs) are data structures that allow efficient searching, insertion, and deletion operations on a collection of elements. They are based on the concept of a binary tree, where each node has at most two children. In a BST, the left child of a node contains elements that are smaller than the node, and the right child contains elements that are greater. This property allows for efficient searching, as comparisons can be made to determine which branch to traverse. Insertions and deletions maintain the BST property by re-arranging the nodes as necessary. BSTs are commonly used in applications such as searching, sorting, and indexing.

## Task 2

- Refer to the following link.
  https://iq.opengenus.org/time-and-space-complexity-of-binary-search-tree/

Discuss the Time and Space complexity of Binary Search Tree (BST) operations (Searching, Insertion, Deletion) in the Best case, average case and worst case.

Binary Search Trees (BSTs) have the following time and space complexities:

1. Searching: Best Case: O(1) (when the element being searched is the root node); Average and Worst Case: O(h), where h is the height of the tree. In a balanced tree, the height is log(n), where n is the number of nodes, so the time complexity is O(log n). In an unbalanced tree, the height is n, where n is the number of nodes, so the time complexity is O(n).

2. Insertion: Best Case, Average Case, and Worst Case: O(h), where h is the height of the tree. In a balanced tree, the height is log(n), where n is the number of nodes, so the time complexity is O(log n). In an unbalanced tree, the height is n, where n is the number of nodes, so the time complexity is O(n).

3. Deletion: Best Case, Average Case, and Worst Case: O(h), where h is the height of the tree. In a balanced tree, the height is log(n), where n is the number of nodes, so the time complexity is O(log n). In an unbalanced tree, the height is n, where n is the number of nodes, so the time complexity is O(n).

The space complexity of a BST is O(n), where n is the number of nodes, since each node requires memory to store its data and pointers to its children. In the worst case, when the tree is completely unbalanced, the space complexity can be O(n).


## Task 3

- Explain how the code in ./src/bst.cpp works. Refer to the following link:
  https://www.geeksforgeeks.org/introduction-to-binary-search-tree-data-structure-and-algorithm-tutorials/

// The provided code is a C++ program for inserting nodes into a binary search tree (BST) and printing the nodes in an inorder traversal.

The program first defines a struct node which represents a node in the BST and contains integer key values as well as left and right pointers to child nodes.

The newNode function allocates memory for a new node, initializes its values, and returns a pointer to the new node.

The insert function recursively traverses the BST to find the appropriate location to insert a new node with the given key value. If the tree is empty, the function creates a new node and returns it.

The inorder function performs an inorder traversal of the BST, recursively calling itself on the left child, printing the node's key value, and then calling itself on the right child.

The main function creates a new BST by inserting nodes with the given key values (50, 30, 20, 40, 70, 60, and 80) and then prints the BST in inorder traversal.

## Task 4: Individual (at home)

- Refer to te following link. Explain how In-order Traversal is used to print a binary search tree.
  https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/BinaryTreeTraversal.html#inorder-traversal

//In-order Traversal is a way to traverse a binary tree by visiting each node in a specific order. In the case of a binary search tree, the in-order traversal visits the nodes in ascending order of their keys. Therefore, by performing an in-order traversal of a binary search tree, we can print the keys of the nodes in ascending order.

To perform an in-order traversal, we first recursively traverse the left subtree, then visit the current node, and then recursively traverse the right subtree. By following this process for each node in the tree, we can print the keys in the correct order.

In the context of printing a binary search tree, we can use in-order traversal to print the keys of the nodes in ascending order. This is useful for various applications where we need to access the nodes of the tree in a specific order, such as searching for a specific node or printing the nodes in a certain order.

## Link(s)

- https://cpp.sh/
- https://www.geeksforgeeks.org/binary-search-tree-data-structure/
