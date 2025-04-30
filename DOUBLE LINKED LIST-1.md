# Exp.no: 43
## DOUBLE LINKED LIST-1

### AIM

To write a python program to traverse the elements in doubly linked list.

### ALORITHM 

1. Start the program.

2. Define Node class with:
   item (data), nref (next reference), pref (previous reference).

3. Define DoublyLinkedList class with:
   start_node to track the beginning of the list.
   insert_in_emptylist(data) – inserts if the list is empty.
   insert_at_start(data) – inserts at the beginning.
   insert_at_end(data) – inserts at the end.
   traverse_list() – prints all elements in order.

4. Create object new_linked_list of DoublyLinkedList.

5. Insert elements:

6. Traverse and print the list.

7. Terminate the program.
   
### PROGRAM

```
class Node:
    def __init__(self, data):
        self.item = data
        self.nref = None
        self.pref = None

class DoublyLinkedList:
    def __init__(self):
        self.start_node = None

    def insert_in_emptylist(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
        else:
            print("list is not empty")
            
    def insert_at_start(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
            print("node inserted")
            return
        new_node = Node(data)
        new_node.nref = self.start_node
        self.start_node.pref = new_node
        self.start_node = new_node
        
    def insert_at_end(self, data):
        if self.start_node is None:
            new_node = Node(data)
            self.start_node = new_node
            return
        n = self.start_node
        while n.nref is not None:
            n = n.nref
        new_node = Node(data)
        n.nref = new_node
        new_node.pref = n
        
    def traverse_list(self):
        if self.start_node is None:
            print("List has no element")
            return 
        else:
            n=self.start_node
            while n is not None:
                print(n.item," ")
                n=n.nref
                
new_linked_list = DoublyLinkedList()
new_linked_list.insert_in_emptylist(50)
new_linked_list.insert_at_start(10)
new_linked_list.insert_at_start(5)
new_linked_list.insert_at_start(18)
new_linked_list.insert_at_end(29)
new_linked_list.insert_at_end(39)
new_linked_list.insert_at_end(49)
new_linked_list.traverse_list()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/2d20d443-b1bd-4bda-ae61-701a6f5d4d19)

### RESULT
Thus the python program was successfully created.
