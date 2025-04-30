# Exp.no: 41
## SINGLY LINKED LIST-1

### AIM

To Write a function to traverse the linked list and display it in the following format.

### ALORITHM 

1. Start the program.

2. Define a Node class with data and next.

3. Define SLinkedList class with head and listprint() method.

4. Create an object of SLinkedList.

5. Create three nodes: "Mon", "Tue", "Wed".

6. Link nodes:
   head → "Mon"
   "Mon".next → "Tue"
   "Tue".next → "Wed"

7. Call listprint() to print all node data.

8. Terminate the program.
   
### PROGRAM

```
class Node:
   def __init__(self, data=None):
      self.data = data
      self.next = None

class SLinkedList:
   def __init__(self):
      self.head = None

   def listprint(self):
      printval = self.head
      while printval is not None:
         print (printval.data)
         printval = printval.next

list = SLinkedList()
list.head = Node("Mon")
e2 = Node("Tue")
e3 = Node("Wed")

list.head.next = e2
e2.next = e3

list.listprint()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/099f2744-057e-46fa-a6bd-c3d4b8969855)

### RESULT
Thus the python program was successfully created.
