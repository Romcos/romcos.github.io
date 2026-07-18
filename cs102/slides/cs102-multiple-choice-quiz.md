# CS102 Multiple-Choice Quiz Base

This file contains three multiple-choice questions per top-level lecture HTML file in this semester's slide folder. Each question includes four choices and the correct answer.

## 01-course_intro.html - Course Intro

1. Why do the slides emphasize understanding data structures even when AI can generate code?
   - A. Because AI tools cannot compile Java programs
   - B. Because debugging, adapting, testing, and choosing data structures require understanding
   - C. Because data structures are only useful in interviews
   - D. Because generated code is always slower than handwritten code
   - Answer: B

2. Which pairing best describes the relationship between a data structure and an algorithm?
   - A. A data structure stores or organizes data; an algorithm is a procedure for solving a problem
   - B. A data structure is Java-specific; an algorithm is language-independent
   - C. A data structure is always faster than an algorithm
   - D. A data structure is a loop; an algorithm is a class
   - Answer: A

3. In the string-building demo, why is `StringBuilder` much faster than repeatedly concatenating `String` objects?
   - A. `StringBuilder` automatically sorts characters
   - B. `StringBuilder` avoids repeatedly creating and copying immutable `String` objects
   - C. `StringBuilder` stores characters in the call stack only
   - D. `StringBuilder` uses recursion instead of iteration
   - Answer: B

## 02-java-memory.html - Java Programs Under the Hood

1. What does the Java compiler produce from a `.java` source file?
   - A. Machine-specific executable code
   - B. Java bytecode in a `.class` file
   - C. A heap snapshot
   - D. A JVM installation
   - Answer: B

2. What is stored in a primitive variable's memory location?
   - A. The actual value of the variable
   - B. A pointer to the source file
   - C. A reference to an object on the heap
   - D. The name of the variable as text
   - Answer: A

3. Where are Java arrays stored?
   - A. Always on the call stack
   - B. Always in the source file
   - C. On the heap, in consecutive memory locations
   - D. In bytecode, not memory
   - Answer: C

## 02-recursion.html - Recursion

1. What is the base case in a recursive algorithm?
   - A. The step that makes the problem larger
   - B. The trivial case that can be solved directly
   - C. The final line of the source file
   - D. The stack frame of the caller
   - Answer: B

2. In the recursive factorial function shown in the slides, what is the recursive call for `factorial(n)` when `n > 0`?
   - A. `factorial(n + 1)`
   - B. `factorial(0)`
   - C. `factorial(n - 1)`
   - D. `factorial(n * n)`
   - Answer: C

3. Which statement about recursion and iteration matches the slides?
   - A. Any problem solved recursively can also be solved iteratively, and vice versa
   - B. Recursive algorithms never use memory
   - C. Recursive implementations are always faster than iterative ones
   - D. Iteration cannot be used for linked lists
   - Answer: A

## 03-data_structures_overview_1.html - Data Structures and Algorithms Overview

1. Why is binary search asymptotically faster than linear search on sorted data?
   - A. It checks every element twice
   - B. It repeatedly halves the remaining search space
   - C. It stores data in a linked list
   - D. It avoids comparisons entirely
   - Answer: B

2. What is the time complexity of accessing an element by index in an array?
   - A. `O(1)`
   - B. `O(log N)`
   - C. `O(N)`
   - D. `O(N^2)`
   - Answer: A

3. Why is binary search generally not efficient on a linked list?
   - A. Linked lists cannot store sorted data
   - B. Linked lists cannot contain numbers
   - C. Accessing an arbitrary middle element takes linear time
   - D. Linked lists must be circular
   - Answer: C

## 03-lists_1.html - Lists Part 1

1. What is an abstract data type (ADT)?
   - A. A precise specification of values and operations, independent of implementation
   - B. A Java class that must use arrays
   - C. A data type that cannot be implemented
   - D. A method for drawing memory diagrams
   - Answer: A

2. In a singly linked list with a `tail` reference, what is the time complexity of adding to the back?
   - A. `O(1)`
   - B. `O(log N)`
   - C. `O(N)`
   - D. `O(N^2)`
   - Answer: A

3. Why does searching a linked list take `O(N)` time in the worst case?
   - A. The list must be resized first
   - B. Each node may need to be visited one at a time
   - C. Every node stores two values
   - D. The list is always unsorted
   - Answer: B

## 04-lists_2.html - Doubly Linked Lists

1. What extra reference does each node in a doubly linked list usually store compared with a singly linked list?
   - A. A reference to the array capacity
   - B. A reference to the previous node
   - C. A reference to the JVM stack frame
   - D. A reference to the list's hash code
   - Answer: B

2. Why is using an iterator preferable to repeated `get(i)` calls when traversing a linked list?
   - A. Iterators sort the list while traversing
   - B. Iterators can visit each node once in `O(N)` time
   - C. Iterators convert the list into an array first
   - D. Iterators avoid storing references
   - Answer: B

3. In a circular linked list, what makes the list circular?
   - A. The first node stores the list size
   - B. The last node's next reference points back to the first node
   - C. Every node stores a duplicate value
   - D. The list cannot be empty
   - Answer: B

## 04-lists_arraylist.html - ArrayList

1. What is the difference between an `ArrayList`'s size and capacity?
   - A. Size is the array length; capacity is the number of stored elements
   - B. Size is the number of stored elements; capacity is the length of the underlying array
   - C. They are always equal
   - D. Capacity counts only non-null values after index 0
   - Answer: B

2. What is the amortized time complexity of appending to an `ArrayList` when the backing array grows by multiplication?
   - A. `O(1)`
   - B. `O(log N)`
   - C. `O(N)`
   - D. `O(N^2)`
   - Answer: A

3. Why is adding or removing at an arbitrary position in an `ArrayList` usually `O(N)`?
   - A. Elements may need to be shifted to preserve order
   - B. Java must recompile the class
   - C. The list must be converted into a linked list
   - D. The hash code must be recomputed for every element
   - Answer: A

## 05-stacks_queues.html - Stacks and Queues

1. Which access rule describes a stack?
   - A. First in, first out
   - B. Last in, first out
   - C. Random access by index
   - D. Highest priority first
   - Answer: B

2. Which access rule describes a queue?
   - A. First in, first out
   - B. Last in, first out
   - C. Smallest key first
   - D. Left child before right child
   - Answer: A

3. Why do circular-array queue implementations use modulo arithmetic?
   - A. To sort queue elements
   - B. To wrap front and rear indexes back to the beginning of the array
   - C. To detect duplicate values
   - D. To convert a queue into a stack
   - Answer: B

## 06-arithmetic_expression.html - Arithmetic Expressions and Problem Solving

1. Why is a stack useful for validating expressions with multiple types of brackets?
   - A. It remembers the most recent unmatched opening bracket
   - B. It converts every bracket into an integer
   - C. It sorts the brackets alphabetically
   - D. It guarantees the expression has no operators
   - Answer: A

2. In postfix notation, where does the operator appear?
   - A. Before its operands
   - B. Between its operands
   - C. After its operands
   - D. On a separate line from its operands
   - Answer: C

3. What is the purpose of Dijkstra's Shunting Yard algorithm in these slides?
   - A. To convert infix expressions to postfix notation
   - B. To balance an AVL tree
   - C. To resize an array queue
   - D. To find connected components in a graph
   - Answer: A

## 06-trees.html - Trees Introduction

1. How is the height of a tree defined in the slides?
   - A. The number of leaves in the tree
   - B. The height of the root, calculated from leaves upward
   - C. The number of edges in the entire graph
   - D. The number of children of the root
   - Answer: B

2. What order does an inorder traversal of a binary tree use?
   - A. Node, left subtree, right subtree
   - B. Left subtree, right subtree, node
   - C. Left subtree, node, right subtree
   - D. Right subtree, node, left subtree, left subtree again
   - Answer: C

3. What data structure does the iterative tree-size algorithm in the slides use to remember unexplored nodes?
   - A. A stack
   - B. A hash table
   - C. A sorted array
   - D. A priority queue
   - Answer: A

## 07-bst.html - Binary Search Trees

1. What property must hold at every node in a binary search tree?
   - A. All values in the left subtree are smaller, and all values in the right subtree are larger
   - B. Every node has exactly two children
   - C. All leaves must be at the same depth
   - D. The tree must be stored in an array
   - Answer: A

2. What is the time complexity of `find` in a BST in terms of tree height `H`?
   - A. `O(1)`
   - B. `O(log H)`
   - C. `O(H)`
   - D. `O(N^2)`
   - Answer: C

3. When removing a BST node with two children, what value can replace it while preserving the BST property?
   - A. Any leaf in the tree
   - B. Its inorder predecessor or inorder successor
   - C. The root value, regardless of position
   - D. The first value inserted into the tree
   - Answer: B

## 09-priority_queues.html - Priority Queues

1. How does `dequeue()` differ in a priority queue compared with a regular FIFO queue?
   - A. It removes the oldest element
   - B. It removes the element with highest priority
   - C. It removes the newest element
   - D. It removes a random element
   - Answer: B

2. What two properties must a binary heap maintain?
   - A. Shape property and heap order property
   - B. BST property and AVL balance factor
   - C. Hash property and load factor
   - D. Inorder property and recursion property
   - Answer: A

3. Why are binary heaps commonly implemented using arrays?
   - A. Complete-tree structure lets parent and child positions be computed by index
   - B. Arrays prevent the need for comparisons
   - C. Arrays make every operation `O(1)` in the worst case
   - D. Arrays automatically remove duplicate priorities
   - Answer: A

## 10-sorting.html - Sorting

1. Which sorting algorithms are described as quadratic sorts in the slides?
   - A. Merge sort, quick sort, and heap sort
   - B. Bubble sort, selection sort, and insertion sort
   - C. Binary search, DFS, and BFS
   - D. Hashing, chaining, and probing
   - Answer: B

2. Why does merge sort run in `O(n log n)` time?
   - A. Each level does `O(n)` merging work and there are `O(log n)` levels
   - B. It never compares values
   - C. It only works on arrays of size 2
   - D. It uses a hash table for every comparison
   - Answer: A

3. What can make quick sort deteriorate to `O(n^2)` time?
   - A. Choosing pivots that split the array very unevenly
   - B. Using recursion at all
   - C. Sorting integers rather than strings
   - D. Using a base case
   - Answer: A

## 12-balanced-bst.html - Balanced BST

1. Why do we want a BST to remain balanced?
   - A. To guarantee traversals take `O(1)` time
   - B. To keep find, add, and remove operations at `O(log N)` in the worst case
   - C. To make every node have two children
   - D. To avoid using comparisons
   - Answer: B

2. What is the AVL tree balance requirement?
   - A. Every node must have balance factor exactly 0
   - B. The heights of the two subtrees of any node cannot differ by more than 1
   - C. The tree must be a complete binary tree
   - D. The root must always be the median of all inserted values
   - Answer: B

3. What is the cost of one AVL rotation according to the slides?
   - A. `O(1)`
   - B. `O(log N)`
   - C. `O(N)`
   - D. `O(N log N)`
   - Answer: A

## 13-hashtables.html - Hash Tables

1. In a dictionary or map ADT, what is true about keys?
   - A. Keys must be stored in sorted order
   - B. Keys are unique, and each key maps to at most one value
   - C. Keys must be integers
   - D. Keys are removed automatically after lookup
   - Answer: B

2. What is a hash collision?
   - A. A key maps to an array index outside the table
   - B. Two different keys map to the same table index
   - C. A table has no empty cells
   - D. A value is larger than its key
   - Answer: B

3. What does rehashing do when a hash table becomes too full?
   - A. Sorts keys alphabetically
   - B. Recomputes all stored positions for a larger table
   - C. Deletes all collisions
   - D. Converts all values into strings
   - Answer: B

## 14-graphs.html - Graphs Introduction

1. What is a graph made of?
   - A. Vertices and edges
   - B. Only arrays and indexes
   - C. Stack frames and heap objects
   - D. Keys and values only
   - Answer: A

2. Which representation stores, for each node, a list of adjacent nodes?
   - A. Edge list
   - B. Adjacency matrix
   - C. Adjacency list
   - D. Implicit heap
   - Answer: C

3. What is the main behavioral difference between DFS and BFS?
   - A. DFS follows paths deeply before backtracking; BFS visits nodes by increasing distance from the start
   - B. DFS only works on weighted graphs; BFS only works on trees
   - C. DFS requires an adjacency matrix; BFS requires an edge list
   - D. DFS is `O(1)`; BFS is `O(N^2)` for all graphs
   - Answer: A
