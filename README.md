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
* 

When I looked at the Shuffle project I thought there were two obvious possibilities for what data structure I could use. The two choices that I decided between was a linked-list and an array based queue. The deciding factor of what data structure to use came down to the question of type of shuffle I wanted to implement. I decided that I wanted to implement the standard riffle shuffle. My reasoning for this type of shuffle was because this is the way I shuffle when I play cards and it was therefore the easiest for me to visualize. After deciding what type of shuffling I wanted I felt that an array-based queue was the best option for me.
	I felt an array-based queue was a better choice than a linked list because I was doing a riffle shuffle. The riffle shuffle involves cutting the deck of cards in close to half and then combining the two separate decks back into one deck by adding one card or multiple cards at a time. I felt this would be easiest because all I would have to do would be to create one array with 52 cards in it. Then I could randomize where I cut the deck, so that it’s not exactly in half every time. Then I would have two separate decks. With those two decks I would use the randomize function to determine from which deck and how many cards would be added to the one combined deck again. The reason I picked an array queue over linked list was because adding and removing in a linked list is O(n) unless it is at the beginning or end of the linked list. While adding and removing on a queue is O(1) unless it needs to grow. But if you allocate the array to be size 52 in the beginning then there really shouldn’t be a reason to ever make it grow. Had I chosen to do another type of shuffle? Some of the tradeoffs had I used a linked list would have been that I could have possibly done it at close to the same speed if I had two linked lists(decks) feeding into one shuffled deck, if I had always added and removed from the top or bottom of the decks. Over all though the linked list would have been much more useful had I decided to implement a Hindu shuffle. It would be a better choice for a Hindu shuffle because in the Hindu shuffle you’re consistently adding or splicing multiple cards into the middle of a deck. Therefore it would have been easy and quicker to just splice in multiple cards in a linked list deck then doing it in a queue.
	Over all I am pleased with my choice to do a queue, but I could also the how using a linked list could be very useful and easy to implement as well.


When looking at the vice project I came down to two different data structures I would use to try to complete the project. I came down to the decision of using an adjacency list or a 1-D array.  Reasons for picking a 1-D array of pointers would have been that once the array is initialized it would be constant time for everything from then on. You wouldn’t need to grow the array once every node is initialized because the size of the board isn’t changing. The positives for the 1-D array would be that it could be fast random access if you found a way to know exactly what node to jump to. The find() and get() functions could be very fast if you somehow used some math to make it so your program knew what node to find. Although the playing field is only 20X20 so it probably wouldn’t be a huge deal if you had to iterate through. Some negatives from using an array of nodes would be that it would take O(n) time to initialize the list. Another con could be that if you didn’t make up some fancy math to be able to random access the specified node you would have to iterate through the array to find it, and that would obviously take some time. If I used a 1-D array my vice game would take a lot of time to create the board. But once the board was created it would be very quick at finding nodes if you used the correct math.
	Positives to using the adjacency list would be that it could easily remember what all of the neighbors of a specific node would be.  Therefore you could easily find neighbors which would make checking for a vice a lot easier and faster than having to iterate through an array to see if a node had a neighbor. Another positive of the adjacency list is that it doesn’t take a ton of memory. Over all the thought of using an adjacency list just made the most sense to me, I could have all of the hex’s or nodes that make up the left side be the main blocks of the adjacency list and I could have everything to their right be in their buckets. Some of the negatives of an adjacency list would be trying to figure out which hex’s to have in a specific bucket since they aren’t straight lines across. Other negatives to using an adjacency list would be having to iterate though the list to find if two nodes were neighbors that could take up to deg(v). If I used adjacency lists my vice game would probably be better and faster at creating the over all board but it would be worse at checking to see if two nodes were neighbors if not implemented really well.
	Over all I am not sure I see a clear cut winner in which one of these data structures would be better to implement. I personally would probably use a 1 or 2-D array to keep track of all the hex’s and their neighbors.
	
	

