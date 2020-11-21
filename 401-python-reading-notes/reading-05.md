[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

A linked list is a sequence of nodes that are connected. There are two types of linked lists, singly and doubly.

singly -  Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

node - nodes are the individual items/links that live in a linked list. Each ode contains the data for each link.

[What's a linked list? pt1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

It can be helpful to think of linked lists and arrays as similar data structures. In both structures, order matters.

Linked lists memory bytes can be stored anywhere.

a node needs to store two things, its data and where to go to find the next bit of data. Doubly linked lists store directional data in both the front and back of the node, so you can go forward or backward through the node chain.

[What's a linked list? pt2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

linked lists pros and cons
pros:
inserting and deleting can be really fast
<br>
dynamic size can grow and shrink easily
<br>
only allocates resources as required at runtime, using non-contiguous chunks of memory as needed.
Helpful of you dont know the size of the list, and mostly want to add or remove things quickly without random access.
<br>
cons:
searching is slow
<br>
finding elements requires traversal, and traversal is slow since you can use binary search.

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)