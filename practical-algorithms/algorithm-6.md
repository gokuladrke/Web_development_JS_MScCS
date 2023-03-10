# Algorithm:

1. Create a new node with the specified data to insert.
2. If the linked list is empty (head is null), set the head to the new node.
3. If the linked list is not empty, set both a slow pointer and a fast pointer to the head node.
4. Traverse the linked list with the fast pointer moving two nodes at a time and the slow pointer moving one node at a time until the end of the list is reached or the fast pointer reaches the end.
5. Set the next pointer of the new node to the next pointer of the slow pointer.
6. Set the next pointer of the slow pointer to the new node.
