# Activities

## Task 1

- Refer to the following link. Discuss how Min Heap data structure works:
  https://www.cs.usfca.edu/~galles/visualization/Heap.html

// A Min Heap is a binary tree data structure where each node's value is less than or equal to its children's values. In other words, the root node has the minimum value among all nodes in the heap. The heap is represented as an array, where the root is at index 0, and for any node i, its left child is at index 2i+1 and its right child is at index 2i+2.

The Min Heap data structure supports two main operations, insertion and extraction of the minimum element. When inserting an element, we add it to the end of the array and compare its value with its parent. If its value is less than its parent's value, we swap the two nodes. We continue doing this until the element is in its correct position.

When extracting the minimum element, we remove the root node and replace it with the last element in the heap. We then compare this element with its children and swap it with the smallest child until it is in the correct position. This process is called heapifying down.

The time complexity of insertion and extraction operations is O(log n), where n is the number of elements in the heap. The space complexity of the Min Heap is O(n), where n is the number of elements in the heap.

## Task 2

- Refer to the following link.
  https://iq.opengenus.org/time-and-space-complexity-of-heap/

Discuss the Time and Space Complexity of Heap data structure operations, in the Best case, average case and worst case.

Time Complexity:

1. Insertion: In the worst-case scenario, when the Heap is full, inserting an element into the Heap will take O(log n) time, where n is the number of elements in the Heap. In the best-case scenario, when the Heap is empty, the insertion operation takes O(1) constant time. In the average case, the time complexity is also O(log n).

2. Deletion: In the worst-case scenario, when the Heap is completely unbalanced, deleting the maximum element from the Heap will take O(n) time. However, in the best-case scenario, when the Heap is perfectly balanced, the deletion operation will take O(log n) time. In the average case, the time complexity is also O(log n).

3. Searching: Searching an element in a Heap takes O(n) time in the worst-case scenario, as all elements may need to be searched to find the desired element. In the best-case scenario, when the element is located at the root of the Heap, the search operation takes O(1) constant time. In the average case, the time complexity is also O(n).

Space Complexity:

1. The space complexity of a Heap is O(n), where n is the number of elements in the Heap. This is because each element in the Heap takes up a constant amount of space, and the maximum number of elements that a Heap can hold is n.

In summary, Heap data structure operations have a time complexity of O(log n) in the best and average cases, and O(n) in the worst case for searching and deletion operations. The insertion operation has a time complexity of O(1) in the best case and O(log n) in the average and worst cases. The space complexity of Heap operations is O(n).

## Task 3

- Explain how the code in ./src/priority-queue.cpp works. Refer to the following link:
  https://www.geeksforgeeks.org/priority-queue-using-binary-heap/

  This C++ code implements a priority queue using an array-based implementation of a binary heap. A binary heap is a complete binary tree where each node is smaller than its children (in a min-heap) or larger than its children (in a max-heap). In this implementation, the maximum priority element is at the root of the binary heap.

The implementation contains the following functions:

*parent(i)*: returns the index of the parent node of a given node i.
*leftChild(i)*: returns the index of the left child of a given node i.
*rightChild(i)*: returns the index of the right child of a given node i.
*shiftUp(i)*: shifts the node at index i up the binary heap to maintain the heap property.
*shiftDown(i)*: shifts the node at index i down the binary heap to maintain the heap property.
*insert(p)*: inserts a new element p into the binary heap.
*extractMax()*: extracts the element with the maximum priority from the binary heap.
*changePriority(i, p)*: changes the priority of an element at index i to a new priority p.
*getMax()*: returns the maximum priority element.
*remove(i)*: removes the element at index i from the binary heap.

The driver code creates a priority queue represented as a binary max-heap array, inserts elements into the priority queue, extracts the element with the maximum priority, changes the priority of an element, and removes an element from the priority queue. The priority queue is printed before and after these operations are performed.

Overall, this code implements a basic priority queue using an array-based implementation of a binary heap. The time complexity of the insert, extractMax, changePriority, and remove operations is O(log n) in the worst case, where n is the number of elements in the priority queue. The space complexity of the implementation is O(n)

## Task 4: Individual (at home)

- Explain how the code in ./src/heap.cpp works. Refer to the following link:
  https://www.geeksforgeeks.org/binary-heap/

  //A min heap is a binary tree where the value of each node is smaller than or equal to its children. The smallest value is at the root of the tree.

The MinHeap class contains private member variables that point to the array of elements in the heap, the maximum possible size of the heap, and the current number of elements in the heap.

The public member functions of the MinHeap class include:

 $The constructor MinHeap(int capacity) initializes the heap size to 0 and allocates memory for the heap array with the given capacity.

 $The insertKey(int k) function inserts a new element into the heap, at the end of the array, and then moves the element up the tree if necessary to maintain the min heap property.

 $The decreaseKey(int i, int new_val) function decreases the value of the element at the given index i to new_val, and then moves the element up the tree if necessary to maintain the min heap property.

 $The extractMin() function removes and returns the minimum element in the heap, which is the root of the tree. It then replaces the root with the last element in the array and moves the new root down the tree if necessary to maintain the min heap property.

 $The deleteKey(int i) function deletes the element at the given index i by first decreasing its value to negative infinity using the decreaseKey() function, and then removing it using the extractMin() function.

 $The getMin() function returns the minimum element in the heap, which is the root of the tree.

 $The MinHeapify(int i) function is a recursive helper function that maintains the min heap property by comparing the parent node with its left and right child nodes, and swapping values if necessary to ensure the smallest value is at the root.
 
The main function creates an instance of the MinHeap class with a capacity of 11, inserts some values into the heap, deletes one value, extracts the minimum value, decreases the value of one element, and prints the new minimum value.

## Link(s)

- https://cpp.sh/
- https://www.geeksforgeeks.org/array-representation-of-binary-heap/
