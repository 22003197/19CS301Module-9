# Exp.no: 43
## ADVANCED LIST PROCESSING

### AIM

To write a python program to find the transpose of a matrix using list Comprehension

### ALORITHM 

1. Start the program.

2. Read the number of rows and columns, convert to integers.

3. Call create_matrix(r, c) to:
   Initialize an empty matrix M.
   Loop through r rows:
   For each row, loop through c columns:
   Read an integer and append to the row.
   Append the row to the matrix M.
   Return the matrix M.

4. Assign the returned matrix to variable A.

5. Print matrix A.

6. Swap rows and columns of matrix A.

7. Print transpose matrix T.

8. Terminate the program.
   
### PROGRAM

```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M 
    
r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
print(A)
T = [[r[i] for r in A] for i in range(len(A[0]))]
print(T)
```

### OUTPUT

![image](https://github.com/user-attachments/assets/a88c8dac-105f-4af8-a280-64d5257a87d8)

### RESULT
Thus the python program was successfully created.
