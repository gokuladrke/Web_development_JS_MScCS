Linked Lists

What is a Linked List?

A linked list is a linear data structure that consists of a sequence of nodes, each containing a data element and a reference to the next node. The order of the nodes is determined by the references between them. Linked lists can be used to implement various abstract data types (ADTs), such as stacks, queues, and associative arrays.

Linked List ADTs

The following basic operations are typically supported by linked list ADTs:

Inserting an element
Deleting an element
Searching for an element
Traversing the list
Linked lists are often used instead of arrays because of their flexibility in size and efficient insertion and deletion operations.

Advantages and Disadvantages of Linked Lists

Advantages:

Dynamic size: Linked lists can grow or shrink in size during runtime, unlike arrays which have a fixed size.
Efficient insertion and deletion: Insertion and deletion can be done with constant time complexity if the position of the element is known.
Sequential access: Traversing the linked list can be done in linear time, allowing for efficient sequential access.
Disadvantages:

Random access: Random access to a particular element in the list is not possible. To access an element, the list must be traversed from the beginning or end.
Extra memory: Linked lists require extra memory to store the reference to the next element.
Overhead: Linked lists have additional overhead compared to arrays due to the storage of pointers or references to the next element.
Singly Linked Lists

Creation and Traversal

To create a singly linked list, we start by creating a head node which contains the first data element and a reference to the next node (initially null). Then, we can add more nodes to the list by creating new nodes and setting the reference of the previous node to the new node. To traverse a singly linked list, we start at the head node and follow the references to the next nodes until we reach the end of the list (when the reference is null).

Singly Linked List Insertion

Inserting a new node at the beginning of the list involves creating a new node, setting its next reference to the current head node, and updating the head to point to the new node.

Inserting a new node at the end of the list involves creating a new node, setting the next reference of the current last node to the new node, and updating the tail to point to the new node.

Inserting a new node in the middle of the list involves finding the node that will precede the new node, setting the next reference of the new node to the next reference of the preceding node, and setting the next reference of the preceding node to the new node.

Singly Linked List Deletion

Deleting the node at the beginning of the list involves updating the head to point to the next node and deallocating the memory of the deleted node.

Deleting the node at the end of the list involves finding the node that precedes the last node, setting its next reference to null, and updating the tail to point to the preceding node. Then, we can deallocate the memory of the deleted node.

Deleting a node in the middle of the list involves finding the preceding node and updating its next reference to skip the node to be deleted. Then, we can deallocate the memory of the deleted node.
