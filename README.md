# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
i.L AND U MATRIX

1.Input the Matrix:

2.Take a square or rectangular matrix as input (the user provides it). The matrix should be in the form of a 2D array.
Convert the input to a NumPy array using np.array(eval(input())).
LU Decomposition:

3.Use the lu() function from scipy.linalg to perform LU decomposition of the input matrix.
The lu() function decomposes the matrix into three components:
piv: The permutation matrix, which represents row swaps (pivoting).
l_matrix: The lower triangular matrix (with diagonal elements as 1).
u_matrix: The upper triangular matrix.
Output the Results:

4.Print the lower triangular matrix (l_matrix).
5.Print the upper triangular matrix (u_matrix).

ii.LU DECOMPOSITION

1.Input the Matrix and Vector:

2.Take a square matrix (matrix) as input, provided in the form of a 2D array.

3.Take a vector (b) as input, which represents the constants in the linear system 
𝐴
𝑥
=
𝑏
Ax=b.

4.LU Factorization:

5.Use the lu_factor() function from scipy.linalg to perform LU decomposition on the matrix.

6.This function decomposes the matrix into a lower triangular matrix 
𝐿

7.L, an upper triangular matrix 
𝑈

8.U, and a pivoting vector for row permutations.
Solve the Linear System:

9.Use the lu_solve() function to solve the linear system 
𝐴
𝑥
=
𝑏
Ax=b, where 
𝐴
A is the input matrix, and 
𝑏
b is the constant vector.
lu_solve() uses the previously computed LU decomposition to find the solution vector 
𝑥
x.
Output the Solution:

10.Print the solution vector 
𝑥
x.


## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by:PANDEESWARAN N
RegisterNumber:24901111
'''
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by:PANDEESWARAN N 
RegisterNumber:24901111
'''

# To print X matrix (solution to the equations)
import numpy as np 
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
b=np.array(eval(input()))
x=lu_factor(matrix)
solution=lu_solve(x,b)
print(solution)
*/
```

## Output:
![result]![Screenshot 2024-11-17 111235](https://github.com/user-attachments/assets/4ecadef2-0a3f-4de7-814c-58fbb2a0e3f1)
![Screenshot 2024-11-17 111310](https://github.com/user-attachments/assets/15a13291-aa39-492e-adf9-cc89cb1395ea)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

