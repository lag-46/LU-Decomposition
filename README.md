# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

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

