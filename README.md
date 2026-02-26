# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Input matrix dimensions and initialize augmented matrix and solution vector.

2.Populate the augmented matrix with user inputs.

3.Perform Gaussian elimination to reduce the matrix to upper triangular form, ensuring no division by zero.

4.Back substitute to compute solution values for the variables.

5.Print the solution vector formatted to two decimal places.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.

import numpy as np
def gauss_elimination(arr,n):
    for i in range(n):
        for j in range(i+1,n):
            ratio=arr[j][i]/arr[i][i]
            for k in range(n+1):
                arr[j][k]-=ratio*arr[i][k]
    x=[0]*n
    for i in range(n-1,-1,-1):
        x[i]=arr[i][n]
        for j in range(i+1,n):
            x[i]-=arr[i][j]*x[j]
        x[i]/=arr[i][i]
    return x
data=[]
n=int(input())
values=[float(input()) for _ in range(n*(n+1))]
idx=0
for i in range(n):
    row=[]
    for j in range(n+1):
        row.append(values[idx])
        idx+=1
    data.append(row)
result=gauss_elimination(data,n)
for i in range(n):
    print(f'X{i} = {result[i]:.2f}',end=' ')


Developed by: LAL RHIDHISHAN.R
RegisterNumber: 25015767
*/
```

## Output:

<img width="1103" height="526" alt="image" src="https://github.com/user-attachments/assets/58a1580d-18a9-4339-9564-4314186a3bfb" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

