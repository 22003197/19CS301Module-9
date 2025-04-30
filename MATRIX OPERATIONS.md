# Exp.no: 41
## MATRIX OPERATIONS

### AIM

To Write a python program to print the only the Diagonal elements of a matrix 

### ALORITHM 

1. Start the program.

2. Read each row of the matrix using input().

3. Convert the row into a list of integers and append it to the matrix.

4. Define print_diagonals(matrix):
   Get the length of the matrix (n).
   Loop through each index i:
   Print spaces (' ') to align the diagonal elements (based on index i).
   Print the element at matrix[i][i] (this is the diagonal element).

5. Print the entire matrix for reference.

6. print the diagonal elements of the matrix.

7. Terminate the program.
   
### PROGRAM

```
def print_diagonals(matrix):
    n = len(matrix)
    for i in range(n):
        for _ in range(i):
            print(' ', end=' ')
        print(matrix[i][i])
rows = int(input())
cols = int(input())
matrix = []
for i in range(rows):
    row = list(map(int, input().split()))
    matrix.append(row)

print(matrix)

print_diagonals(matrix)
```

### OUTPUT

![image](https://github.com/user-attachments/assets/f00db8fc-d318-4462-a999-42aedf8e2261)

### RESULT
Thus the python program was successfully created.
