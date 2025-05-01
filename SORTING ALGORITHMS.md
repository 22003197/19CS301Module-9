# Exp.no: 44
## SORTING ALGORITHMS

### AIM

To type a python function to print this matrix in ZIG-ZAG fashion.

### ALORITHM 

1. Start the program.

2. Read the size of the square matrix.

3. Create matrix:
   Initialize an n x n matrix with zeros.
   For each row, read n integers and fill the matrix.

4. Zigzag traversal:
   Create a list solution with 2n - 1 empty sublists (for diagonals).
   For each element at position (i, j) in the matrix:
   Compute sum = i + j.

5. If sum is even, insert the element at the start of solution[sum].
   If sum is odd, append the element to solution[sum].

6. Print all elements in solution lists in order (zigzag pattern).

7. Terminate the program.
   
### PROGRAM

```
def create_matrix(n):
    matrix = [[0]*n for row in range(n)]
    for i in range(n):
        lines = list(map(int, input().split()))
        for j in range(n):
            matrix[i][j] = lines[j]
    return matrix
def print_zigzag(matrix):
    solution=[[] for i in range(n+n-1)]
    for i in range(n):
        for j in range(n):
            sum=i+j
            if(sum%2 ==0):
              solution[sum].insert(0,matrix[i][j])
            else:
                solution[sum].append(matrix[i][j])
    for i in solution:
        for j in i:
            print(j,end=" ")
    
n= int(input())
M=create_matrix(n)
print_zigzag(M)
```

### OUTPUT

![image](https://github.com/user-attachments/assets/6e927ebd-0d5d-4d7e-b132-d6e5e73b7900)

### RESULT
Thus the python program was successfully created.
