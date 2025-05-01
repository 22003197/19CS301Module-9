# Exp.no: 45
## SEB

### AIM

To write a python program to find the square root of all elements in a list using list comprehension.

### ALORITHM 

1. Start the program.

2. Read the number of elements.

3. Create an empty list.

4. Read n float values – Append each to the list l.

5. Compute square roots – Create a new list sq_l with the square root of each element in l.

6. Print l and sq_l – Display the original and square root lists.

7. Terminate the program.
   
### PROGRAM

```
n=int(input())
l=[]
for i in range(n):
    x=float(input())
    l.append(x)
sq_l=[item**0.5 for item in l]
print(l)
print(sq_l)
```

### OUTPUT

![image](https://github.com/user-attachments/assets/8133ae95-dbbb-4927-9d3f-b265b2c5797d)

### RESULT
Thus the python program was successfully created.
