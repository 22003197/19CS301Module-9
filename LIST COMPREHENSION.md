# Exp.no: 42
## LIST COMPREHENSION

### AIM

To write a Python program to store a scalar multiple of a set of numbers  in a list using list comprehension.

### ALORITHM 

1. Start the program.

2. Read the number of elements to be entered and scaling factor.

3. Create an empty list to store float numbers.

4. For each iteration:
   Read a float number.
   Append the number to list l.

5.  Multiply each element in l by scl and store the results in a new list sq_l.

6.  Print the original list l and the scaled list sq_l.

7. Terminate the program.
   
### PROGRAM

```
n=int(input())
scl=int(input())
l=[]
for i in range(n):
    x=float(input())
    l.append(x)
sq_l=[item*scl for item in l]
print(l)
print(sq_l)
   
```

### OUTPUT

![image](https://github.com/user-attachments/assets/74283904-fabc-4495-84f3-db41cdc6723e)

### RESULT
Thus the python program was successfully created.
