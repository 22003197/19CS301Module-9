# Exp.no: 45
## SEB

### AIM

To write a python program to delete an element from a specific location in the given linked list.

### ALORITHM 

1. Start the program.

2. Create a Node class with:
   data to store value
   next to point to the next node

3. Create a linked list class (delete_front) with:
   head to store the start of the list

4. Define push(data):
   Add new node at the front of the list

5. Define removeNode(position):
   If position is 0 → remove the head node
   Else → move to the node before the position and update its next to skip the target node

6. Print all node values from start to end

7. In main:
   Take input for number of elements
   Insert elements using push()
   Delete node at position 3 using removeNode(3)
   Display the final list using display()

8. Terminate the program.
   
### PROGRAM

```
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
        
class delete_front:
    def __init__(self):
        self.head = None
  
    def removeNode(self, position):
        if self.head==None:
            return
        temp=self.head
        if position ==0:
            self.head=temp.next
            temp=None
            return
        for i in range(position-1):
            temp=temp.next
        temp1=temp.next.next
        temp.next=temp1
        
    def push(self, data):
        if self.head is None:
            self.head = Node(data)
            return
        temp = Node(data)
        temp.next = self.head
        self.head = temp
        
    def display(self):
        temp1 = self.head
        while temp1 is not None:
            print(temp1.data , end =" ")
            temp1 = temp1.next
dfront = delete_front()
val = int(input("Enter the number of elements to push:\n"))
for i in range(val):
    data = int(input())
    dfront.push(data)
dfront.removeNode(3)     
dfront.display()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/1e639ec2-0a5f-469f-aba6-ef6c9d92393a)

### RESULT
Thus the python program was successfully created.
