# **MY SHORT NOTE TO DATA STRUCTURE**
## **Author: [Nuelgeek](https://twitter.com/theNuelgeek) | Software Engr | Smart Contract Developer**

--------------------

**ABOUT :** 
- This note will contain a summary of different data structures, algorithms, and some implementation on typescript. These contents are notes I made up from Data structure classes from Frontend masters.

**AIM :** 
- This note is to help you with snippet of data structure and algorithms meanings and how it works.
  
- It can be useful for preparation of job interview without the hassle of reading voluminous information.

- Looking for straight forward contents on Data structure, this is for you.


-------------

# *! Let's Gooooooooooo*


## What is Data Structure ?
Data structures frame the organization of information so that machines and humans can better understand it.

## What is Alogrithm ?
Algorithm is a step-by-step procedure, which defines a set of instructions to be executed in a certain order to get the desired output.

## What is Big O ?
Big O is a way to categorize your algorithms time or memory requirements based on input. It is not meant to be an exact measurement. It will not tell you how many CPU cycles it takes, instead it is meant to generalize the growth of your algorithm.

## Important Concepts
1.  Growth is with respect to the input
2.  Constants are dropped
3.  Worst case is usually the way we measure
   
   ------
  
# SEARCH

   - **Linear search** is an alorithm technique, where you must traverse through the array's index to obtain a value. 
that is measurable in O(N) . [typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/LinearSearchList.ts)
   - A form of search method called **binary search** involves halving the size of an ordered dataset until the target value is located. Measured in
O(logN) or O(NlogN). [typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BinarySearchList.ts)

-----------

# SORT
-  **Bubble sort** is a type of algorithm where a single iteration produces the largest number (data) at the last index till the dataset is sorted. The next iteration won’t include the last index. It is measured in O(N^2). [typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BubbleSort.ts)
-  **A linked list** is a linear collection of data elements whose order is not given by their physical placement in memory. Instead, each element points to the next. It is a data structure consisting of a collection of nodes which together represent a sequence. Runtime is O(1). 
-  **A Queue** is a specific implementation of a linked list where there is no Bi link to the Node, which is denoted as FIFO (First In First Out) operation. The runtime is N(1). [typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/Queue.ts)
-  **A Stack** is a single-Linked list where we get to add to it and remove from the head, denoted as FILO (First In Last Out). Runtime is O(1). [typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/Stack.ts)

----
# ARRAY

- **Array vs Linked list**
  
| Array | Linked list |
| ----------- | ----------- |
| 1. Access to Indices | Indices don’t exist in the list. |
| 2. It is O(1) when you want to write into an array. | It is O(1) when you want to insert into a listext | 
| 3. You have to allocate the memory of your array up front, even if you’re not aware of the memory length needed.  | Memory are created instantly when a data is added to the node, but it costs a runtime to create the memory. | 
| 4. You have options of search methods in your array. E.g. Binary Search etc  | Linear search is your only option when you want to search for a data in your list. |

- **ArrayList** uses the array as the fundament base to perform extra operations on it like Resizing, Pushing, Popping etc. Array list is time-consuming using Enqueue/Dequeue and fast with Push/Pop.[typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/array-test.ts)
- **Array Buffer**, is used when there is some uncertainty about the amount of data or the rate of arrival of the data that will be placed there.

------
# RECURSION
**Recursion** is a type of algorithm that constantly calls its function until the base case is satisfied, or an action is completed. Understanding your base case will help you comprehend recursion better.

**Three steps make up recursion.**
- Pre; Before recusing, you can do an operation.
- Recuse; Does the calling of the function.
- Post; After recusing, you can execute an operation.

Even if you don't use these stages directly, it's still vital to be aware of them because pathing depends heavily on them.
[MazeSolver algorithm Implementation  to understand recursion](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/MazeSolver.ts)

*Note :*
-  If you have a solid understanding of why you should stop recusing, that reason makes up a solid base case.
-  You might ask when should you use a recursion algorithm instead of loop algorithm?; Answer: When there is no defined end or when there is branching factor.

# QUICK SORT

Divide and conquer is a strategy used by the **QuickSort algorithm**.
The algorithm selects a pivot element and moves the array's elements in such a way that those that are smaller than the pivot element are moved to the left side and those that are greater are moved to the right side.
The subarrays to the left and right of the pivot element are then sorted repeatedly by the algorithm. The running time of this algorithm is O(NlogN) or  O(N^2)

------
# TREE

The tree is a data structure that starts from a single point and goes all down like roots, the computer’s hard drives, its directories and how it is organized is a good illustration of a tree.
A tree is a structure made up of one node called the root and zero, one, or more subtrees. It can also be empty and have no nodes.

# TREE TERMINOLOGY

- **Root:** The most parent node. The First. Adam.
- **Height:** The longest path from the root to the most child node
- **Binary tree:**  A tree in which has at most 2 children, at least 0 children
- **General tree:** A tree with 0 or more children
- **Binary search tree:** A tree in which has a specific ordering to the nodes and at most 2 children
- **Leaves:** A node without children
- **Balanced:** A tree is perfectly balanced when any node's left and right children have the same height.
- **Branching factor:** The amount of children a tree has.
  
# Traversal | Visiting a Node
There are different ways in which you can visit the nodes of a tree.
- Pre order
- In order
- Post order
  
Inorder traversal traverses one subtree of a node, visits the node, and then traverses its other subtree. Preorder traversal visits a node and then traverses both of its subtrees. Postorder traversal traverses both subtrees of a node, then visits the node.
The traversal method makes use of recursion technique while visiting the nodes. The running time of this traversal is O(N). Implementation ([PreOrder](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BTPreOrder.ts), [InOrder](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BTInOrder.ts), [PostOrder](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BTPostOrder.ts)). Note: This type of order is Depth First search | DFS, We implicitly used stack DS for calling the recuse function. 

# TREE SEARCH
**Breath first search:** This is a type of tree search that implicitly makes use of Queue data structure while visiting each node on a tree level. The run time of this data structure is O(N), but if make use of an array list, the run time will be O(N^2). [Breath first search Implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BTBFS.ts). 

- Note: An Interview question example of comparing two binary trees to see if they equal in both shape and structure. Depth-first search preserves tree shape, while breadth-first search does not. [implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/CompareBinaryTrees.ts).

# Heap (priority queue)
Heap data structure as a binary tree, where every child and grandchild is smaller (MinHeap) or larger than (MaxHeap) the current node.

- Whenever a node is added, we must adjust the tree
- Whenever a node is deleted, we must adjust the tree
- There is no traversing in the tree
- Binary is always a complete tree
------------------------
**Some cool characteristics**
- It is self-balancing
- It can be used for priority
- Funnest data structure to implement, but easy to get wrong!

The runtime of this algorithm is O(N log n). [Heap Typescript implementation
](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/MinHeap.ts).

# Tries
A trie is a special tree that can compactly store strings. Also known as radix tree,         prefix tree, digital tree, you can perceive is as an auto complete e.g., when you swipe through your phone keyboard it auto generates a word for you that’s how a trie works. Runtime O(1). 

# Graphs
Graphs are a series of node with some amount of connection or no connection, and they are connected nodes without roots. 

## **Terminology of Graphs**
-----------------------
This is not an exhaustive list of terms, but it is the terms that we may end up using today.

**Graph Terms**

- **cCcle:** When you start at Node(x), follow the links, and end back at Node(x).

- **Acyclic:** A graph that contains no cycles
connected: When every node has a path to another node.

- **Directed:** When there is a direction to the connections. Think Twitter

- **Undirected:** !directed.
Weighted: The edges have a weight associated with them. Think Maps.

- **Dag:** Directed, acyclic graph.

---------------
## **Implementation Terms**
**Node:** a point or vertex on the graph.

**Edge:** the connection betxit two nodes.

----------------

The **BigO** is commonly stated in terms of V and E where V stands for vertices and E stands for edges
So O(V * E) means that we will check every vertex, and on every vertex we check every edge

-------------------------
## **How are graphs represented**
- **Adjacency list:** This is a type of list where the indices map to the node. [DFS on Adjacency list typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/DFSGraphList.ts).

- **Adjacency matrix:** An adjacency matrix is a way of representing a graph as a matrix of booleans (0's and 1's). A finite graph can be represented in the form of a square matrix on a computer. [BFS on Adjacency matrix typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/BFSGraphMatrix.ts).

- **Dijkstra shortest path search:** Dijkstra's shortest path is an algorithm that finds the shortest paths between nodes in a graph. It produces the shortest path tree with the source node as the root. It is profoundly used in computer networks to generate optimal routes with the aim of minimizing routing costs. Runtime is O(logV(V + E)). [Dijkstra implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/DijkstralList.ts).

-------------------------
# Maps & LRU (Least Recently Used)
A Map is a type of fast key lookup data structure that offers a flexible means of indexing into its individual elements.

**Terms**
- **load factor:** The amount of data points vs the amount of storage (data.len / storage.capacity)
- **key:** a value that is hashable and is used to look up data. The hash has to be consistent.
- **Value:** a value that is associated with a key
collision: when 2 keys map to the same cell.

# LRU
The Least Recently Used (LRU) Cache mechanism, allowing you to quickly identify which item hasn't been used for the longest amount of time. An LRU cache is a combination of map and linked list data structures. This algorithm makes use of double linked list & Hash maps. [LRU cache typescript implementation](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/LRU.ts). 

-------------------------

- ## Thanks for reading my note, if you find this note valuable you can give me a follow on twitter [@the_nuelgeek](https://twitter.com/theNuelgeek) and subscribe to email list on hashnode [Geeks Oasis](https://nuelgeek.hashnode.dev/)

- ## You can also make a pull request or contact me, if you have any extra data structure / Alogrithm you want to add.

- ## Contact me for your smart contract development project and smart contract auditng. Next new skill Frontend development.
- ## Feedbacks are highly welcomed.