# DeleteEnd
## A program to delete a node from the end of the singly linked list

In this program, we will create a singly linked list and delete a node from the end of the list. To accomplish this task, we first find out the second last node of the list. Then, make second last node as the new tail of the list. Then, delete the last node of the list.

![](https://static.javatpoint.com/corebasic/programs/images/java-program-to-delete-a-node-from-the-end-of-the-singly-linked-list.png)

Java program to delete a node from the end of the singly linked list
In the above example, Node was the tail of the list. Traverse through the list to find out the second last node which in this case is node 4. Make node 4 as the tail of the list. Node 4's next will point to null.

Algorithm
Create a class Node which has two attributes: data and next. Next is a pointer to the next node in the list.
Create another class DeleteEnd which has two attributes: head and tail.
addNode() will add a new node to the list:
Create a new node.
It first checks, whether the head is equal to null which means the list is empty.
If the list is empty, both head and tail will point to a newly added node.
If the list is not empty, the new node will be added to end of the list such that tail's next will point to a newly added node. This new node will become the new tail of the list.
a. DeleteFromEnd() will delete a node from the end of the list:


It first checks whether the head is null (empty list) then, display the message "List is empty" and return.
If the list is not empty, it will check whether the list has only one node.
If the list has only one node, it will set both head and tail to null.
If the list has more than one node then, traverse through the list till node current points to second last node in the list.
Node current will become the new tail of the list.
Node next to current will be made null to delete the last node.
a. display() will display the nodes present in the list:

Define a node current which will initially point to the head of the list.
Traverse through the list till current points to null.
Display each node by making current to point to node next to it in each iteration.
