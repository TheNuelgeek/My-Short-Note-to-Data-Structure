# **MY SHORT NOTE TO DATA STRUCTURE**
## **Author: [Nuelgeek](https://twitter.com/theNuelgeek) | Software Engr | Smart Contract Developer**

--------------------

**ABOUT :** 
- This note will contain a summary of different TOP(real world used) data structures, algorithms, and some implementation on typescript. These contents are notes I made up from Data structure classes from Frontend masters.

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

## WHat is Big O ?
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
| 2. It is O(1) when you want to write into an array. | It is O(1) when you want to insert into a list | 
| 3. You have to allocate the memory of your array up front, even if you’re not aware of the memory length needed.  | Memory are created instantly when data is added to the node, but it costs a runtime to create the memory. | 
| 4. You have options for search methods in your array. E.g. Binary Search etc  | Linear search is your only option when you want to search for data in your list. |

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
[MazrSolver algorithm to understand recursion](https://github.com/TheNuelgeek/Data-Structure-Algorthim-kata-machine/blob/master/src/day1/MazeSolver.ts)

*Note :*
-  If you have a solid understanding of why you should stop recusing, that reason makes up a solid base case.
-  You might ask when should you use a recursion algorithm instead of loop algorithm?; Answer: When there is not defined end or when there is branching factor.

-----
# QUICK SORT

Divide and conquer is a strategy used by the **QuickSort algorithm**.
The algorithm selects a pivot element and moves the array's elements in such a way that those that are smaller than the pivot element are moved to the left side and those that are greater are moved to the right side.
The subarrays to the left and right of the pivot element are then sorted repeatedly by the algorithm. The running time of this algorithm is O(NlogN)/  O(N^2)

------
# *Up Next: Advanced DSA (Trees, Tree Search, Heap, Graphs, Maps&LRU) So do STAR the repository* 
