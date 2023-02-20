Doubly Linked List

Doubly Linked List Insertion and Deletion

A doubly linked list is a type of linked list where each node has two references, one to the next node and one to the previous node. This allows for traversal in both directions, making it more versatile than a singly linked list.

Insertion
Inserting a new node at the beginning of the list involves creating a new node, setting its next reference to the current head node, and updating the head to point to the new node. The new node's previous reference should be null.

Inserting a new node at the end of the list involves creating a new node, setting its next reference to null and its previous reference to the current last node. The current last node's next reference should be updated to point to the new node, and the new node should become the last node.

Inserting a new node at the middle of the list involves creating a new node and setting its next and previous references to the appropriate nodes. The references of the surrounding nodes should also be updated to include the new node.

Deletion
Deleting a node from the beginning of the list involves updating the head node to point to the next node, setting the previous reference of the new head node to null, and deleting the old head node.

Deleting a node from the end of the list involves updating the previous reference of the current last node to point to the second-to-last node, setting the next reference of the second-to-last node to null, and deleting the old last node.

Deleting a node from the middle of the list involves updating the next and previous references of the surrounding nodes to bypass the node to be deleted, and then deleting the node.
