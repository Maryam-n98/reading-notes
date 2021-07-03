# Read: Linked Lists

### Linked Lists:
 LinkedList is a data structure that stores elements in a non-contiguous location. It is a linear data structure.
 There are two types of Linked List - Singly and Doubly. 

 ###### Singly: 
 The singly linked list is a linear data structure in which each element of the list contains a pointer which points to the next element in the list.

 ###### Doubly:
 are an extension of basic linked lists, but they contain a pointer to the next node as well as the previous node. This ensures that the list can be traversed in both directions.

 ###### Node:
 Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

 ###### Next:
 Each node contains a property called Next. This property contains the reference to the next node.

 ###### Head:
 the first node in a linked list.
 this is effectively the only entry point to the list and all of its elements.
 ###### Current:
 node that is currently being looked at. When traversing.


 ### What’s a Linked List, Anyway? [Part 1]

###### Linear data structures:
in Java is a way to organize the data in the language in a particular way so to use them in the most effective way. The main reason to classify them is that we need less complexity and less space.

Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.

 a dynamic data structure can shrink and grow in memory. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well.

 Parts of a linked list
A linked list can be small or huge, but no matter the size, the parts that make it up are actually fairly simple. A linked list is made up of a series of nodes, which are the elements of the list.

A single node is also pretty simple. It has just two parts: data, or the information that the node contains, and a reference to the next node.

Lists for all shapes and sizes:
Singly linked:
 lists are the simplest type of linked list, based solely on the fact that they only go in one direction. There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.

doubly linked list: This can be helpful if we wanted to be able to traverse our data structure not just in a single track or direction, but also backwards, too.

### What’s a Linked List, Anyway? [Part 2]

##### Big O:
 notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity.

 As far as linked lists go, however, the two types of Big O equations to remember are O(1) and O(n).

 Growing a linked list
We already know what linked lists are made of, and how their non-contiguous memory allocation makes them uniquely different from their seemingly more popular cousin, the array.