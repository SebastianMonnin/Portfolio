Author
==========
"Monnin, Sebastian", monninse
Portfolio
=========

Document completion of the course's learning outcomes.

Instructions
====
The goal of this is to make it very easy for me (or an employer, or a teaching assistant) to see whether or not you have mastered the material of the class. The hope is that I would be able to grade your work without downloading and compiling your code. If you have recorded proper video demonstrations of your programs, that should be sufficient. You will also want to write a paragraph or so making your case for why you deserve full credit for particular learning outcome (or if you don't, then you should say so).

Important
=========
If you prefer, you may turn this in to me via email, instead of hosting it on GitHub. Please talk to me about it during office hours or before or after class.

Body of portfolio
====

7 - Create an implementation of a Queue
----
Possible sources of evidence (do any one of these):

I chose to implement a Queue in the Queue Lab which you can find at the following https://github.com/SebastianMonnin/03_Queue_Lab/tree/monninse

* https://github.com/MiamiOH-CSE274/03_Queue_Lab
* Use a queue as your data structure in https://github.com/MiamiOH-CSE274/Shuffle
* Consult with Dr. Brinkman on an alternative project

7 - Create an implementation of a List

I implemented a List in my Linked List Lab -   https://github.com/MiamiOH-CSE274/04_Linked_List_Lab/tree/monninse 
----
Possible sources of evidence (do any one of these):

* https://github.com/MiamiOH-CSE274/04_Linked_List_Lab
* Use a linked list as your data structure in https://github.com/MiamiOH-CSE274/Shuffle
* Implement chaining instead of linear probing in https://github.com/MiamiOH-CSE274/05_Hashing_Lab
* Consult with Dr. Brinkman on an alternative project


7 - Create an implementation of a Binary Search Tree

I created a BST in my BST lab - https://github.com/SebastianMonnin/06_BST_Lab/tree/monninse
----
Possible sources of evidence (do any one of these):

* Binary Search Tree Lab (TODO)
* Use a binary search tree or KD-Tree in the Starbucks project.
* Use a binary search tree in the Zeitgeist project
* Consult with Dr. Brinkman on an alternative project


7 - Create an implementaiton of a Hash Table

I created a hash table in my hash table lab --> https://github.com/SebastianMonnin/05_Hashing_Lab/tree/monninse
----
Possible sources of evidence (do any one of these):

* https://github.com/MiamiOH-CSE274/05_Hashing_Lab
* Use a hash table in the Zeitgeist project
* Use locality-preserving hashing on the Starbucks project (not recommended!)
* Consult with Dr. Brinkman on an alternative project

7 - Create an implementation of a Heap

I implemented a heap in my heap lab -- https://github.com/SebastianMonnin/07_Heap_Lab/tree/monninse
----
Possible sources of evidence (do any one of these):

* Heap lab (TODO)
* Implement heap sort in the Sorting lab (TODO)
* Implement a heap as part of the Graph Algorithms lab (TODO)
* Implement a heap as part of the Graph Project (TODO)
* Consult with Dr. Brinkman on an alternative project

7 - Create an implementation of either Adjanency Lists or Adjacency Matrices

I created an adjanency list in my graph lab -- https://github.com/SebastianMonnin/08_Graph_Lab/tree/monninse
----
Possible sources of evidence (do any one of these):

* Graph lab
* Graph Algorithms lab
* Graph project
* Consult with Dr. Brinkman on an alternative project

7 - Implement graph algorithms

I implemented a graph algorithm with my graph lab -- https://github.com/SebastianMonnin/08_Graph_Lab/tree/monninse
----
Possible sources of evidence (do any one of these):

* Graph lab
* Graph Algorithms lab
* Graph project
* Consult with Dr. Brinkman on an alternative project

21 - Determine space and time requirements of common data structure methods
-----
Possible sources of evidence (do up to 3 of these, up to 7 points for each):

* Select any of the following labs, and analyze the running times for each of your methods of your data structure: Queue, Linked List, Binary Search Tree, Heap, Hash Table, Graph (Adjacency List or Adjacency Matrix, you don't have to do both, but you can if you want)
* 

Queue- 
1. remove takes O(1) time, it is O(1) time because we are able to jump to the front item in the backing array that is going to be removed. 
2. add takes O(1) time, unless it calls grow O(n) as long as numItems doesn't equal the backing arraysize you are able to add items to the back of the array in constant time, if numItems=backingarraysize then it takes O(n) time because you have to grow the array to make more space
4. grow takes O(n) time. The reason for this is because every item in the original backing array must be iterated through to copy it to the bigger array
5. getNumItems is O(1) time. Reason being that all it has to do is return numItems

Linked List-
1. Add takes O(1) if i==0 or if i==size()-1 otherwise is O(n). The reason for this is that at the start or end of the linked list it find doesn't have to iterate through. Therefore add can only go as fast as find() works
2. remove takes O(1) if i==0 or if i==size()-1 otherwise is O(n)  The reason for this is that at the start or end of the linked list it find doesn't have to iterate through. Therefore remove() can only go as fast as find() works
3. get  takes O(1) if i==0 or if i==size()-1 otherwise is O(n)  The reason for this is that at the start or end of the linked list it find doesn't have to iterate through. Therefore get() can only go as fast as find() works
4. set  takes O(1) if i==0 or if i==size()-1 otherwise is O(n)  The reason for this is that at the start or end of the linked list it find doesn't have to iterate through. Therefore set() can only go as fast as find() works
5. size() is O(1) time. Reason for this being that it is only one line that is returning a variable
6. find takes O(1) if i==0 or if i==size()-1 otherwise is O(n) Find() takes O(1) when the item that needs to be found is at the front or back of the linked list because it would have to iterate through to find it. Otherwise find() must iterate through the entire linked list which takes O(n) time

HashTable
1. keyExists is O(1). Reason being everything in the method is linear
2. find is O(1). Reason being no loops, everything is linear
3. remove is O(1), Reason being that everything is constant time
4. size is O(1). Reason being that it is just returning a variable
5. add should be reasonably fast O(1). Use linear probing to find an open slot in the hash table. This will be O(1), on average, except when grow is called then it will be O(n)
6. grow should be O(n). Reason being that


5 - Describe memory management in C++, and correctly use dynamic variables, including destructors
----
Possible sources of evidence (do one):

* Select any of your labs or projects that uses dynamic memory, and explain how memory is managed. In particular, you must show that your program does not leak memory, and does not suffer from dangling pointers or out of bounds array access. This will probably require referring to your code, providing links.
* 

https://github.com/SebastianMonnin/04_Linked_List_Lab/blob/monninse/LinkedList.ipp

In my linked list lab memory is managed through the C++ concept of pointers. Each node that is created to make the linked list is a pointer. The origina dummy node is created in the memory by the constructor using the keyword new. After that the add() method is used to create and add other nodes to the linked list which is created in memory. When the remove method is called the item that is to be removed is deleted and the items around it are linked together. To completely delete the linked list you use the destructor. It iterates through the linked list deleting each node and then finally deleting the dummynode. 


5 - Create collection classes using templates in C++
----

 Heap Lab --> https://github.com/SebastianMonnin/07_Heap_Lab/blob/monninse/Heap.ipp
 
 The reasoning behind using templates is because it makes code more reuseable and generic. This helps in the long run because it makes it so we don't have to make specific functions and classes for specific arguments.Templates were used in my heap lab because all of the my functions are template functions. This makes it so each function can accept different types of arguments and not crash. Two types of templates are used in each function, Pri and T, Pri is the priority queue that the heap is built on and T is the data template, it holds the information. 
 
Possible sources of evidence (do one):

* Any of the labs or projects, provided it uses templates in an interesting way.


30 - Using time and space analysis, justify the selection of a data structure for a given application
----

Possible sources of evidence (do up to 2 of these, up to 15 points for each):

* Select a project for which there are multiple reasonable data structure designs. Describe two reasonable options, and explain the trade-offs between them. For each, describe an application where the data structure would be better. For example, if comparing KD-Trees to a Grid in the Starbucks problem, which one is better really depends on the input data set. Explain what the data would have to look like for the Grid to be a clear winner, and also what type of data would lead you to use a KD-Tree instead.
