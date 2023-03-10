# Algorithm:

1. Check if the linked list is not empty by checking if the head node is not null.
2. If the linked list is not empty, check if there is only one node in the linked list by checking if the next node after the head is null.
3. If there is only one node in the linked list, set the head to null to delete the tail element.
4. If there is more than one node in the linked list, traverse the list until the second to last node is reached by setting current to head and looping while current.next.next is not null.
5. Set the next pointer of the second to last node to null to delete the tail element.
