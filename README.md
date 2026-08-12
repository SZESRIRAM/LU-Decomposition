# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix
Step 1 :
Import the required libraries os, numpy, and scipy.linalg.
Step 2:
Get the matrix as input and convert it into a NumPy array using np.array().
Step 3:
Using the lu() function, we get three results: permutation matrix P, lower triangular matrix L, and upper triangular matrix U.
Step 4:
Print the L and U matrices.

(ii) To find the LU Decomposition of a Matrix
Step 1 :
Get the coefficient matrix A and right-hand-side matrix/vector B as input.
Step 2:
Convert the input matrices into lists and import lu_factor() and lu_solve() from scipy.linalg.
Step 3:
Using lu_factor(), perform LU factorization of matrix A and obtain the LU matrix and pivot information.
Step 4:
Using lu_solve(), solve the system of equations and print the solution x.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Ponsriram P
RegisterNumber: 212225240105
import os
os.environ['OPENBLAS_NUM_THREADS']='1'
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Ponsriram P
RegisterNumber: 212225240105
a=eval(input())
b=eval(input())
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
a=list(a)
b=list(b)
from scipy.linalg import lu_factor,lu_solve
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
*/
```

## Output:
(i) To find the L and U matrix
<img width="1152" height="383" alt="image" src="https://github.com/user-attachments/assets/2760aec6-cf35-4619-bea5-afd621a19251" />

(ii) To find the LU Decomposition of a matrix
<img width="864" height="129" alt="image" src="https://github.com/user-attachments/assets/b0ca9e5a-9214-41fd-945c-9fc79a87ee3e" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

