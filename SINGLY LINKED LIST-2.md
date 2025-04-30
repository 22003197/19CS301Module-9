# Exp.no: 42
## SINGLY LINKED LIST-2

### AIM

To write a python program to add new element at the start of the list.

### ALORITHM 

1. Start the program.

2. Define Node class with data and next.

3. Define LinkedList class with head and methods:
   push_front(): Inserts new node at the beginning.
   PrintList(): Traverses and prints the list.

4. Create a LinkedList object named MyList.

5. Insert elements using push_front().

6. Print the list using PrintList().

7. Terminate the program.
   
### PROGRAM

```
class Node:
  def __init__(self, data):
    self.data = data
    self.next = None

class LinkedList:
  def __init__(self):
    self.head = None

  def push_front(self, newElement):
    
    newNode=Node(newElement)
    newNode.next=self.head
    self.head=newNode

  def PrintList(self):
    temp = self.head
    if(temp != None):
      print("The list contains:", end=" ")
      while (temp != None):
        print(temp.data, end=" ")
        temp = temp.next
      print()
    else:
      print("The list is empty.")

MyList = LinkedList()

MyList.push_front(10)
MyList.push_front(20)
MyList.push_front(30)
MyList.PrintList()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/fa4f51bf-a226-4c44-8579-1fae56dca472)

### RESULT
Thus the python program was successfully created.
