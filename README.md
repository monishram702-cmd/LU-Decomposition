# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input matrix (and right-hand side vector for solving equations) from the user.
2. Convert the given input into a NumPy array.
3. Apply LU decomposition to factorize the matrix into Lower triangular matrix (L) and Upper triangular matrix (U).
4. Display the L and U matrices, and if required, solve the system of linear equations using the decomposed matrices.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Monish.R
RegisterNumber: 212225230185
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Monish.R
RegisterNumber: 212225230185
*/

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
```

## Output:
<img width="1231" height="485" alt="Screenshot 2026-02-26 143620" src="https://github.com/user-attachments/assets/cd14c204-2ed2-49c9-9c25-7794880fab92" />
<img width="1258" height="334" alt="Screenshot 2026-02-26 143637" src="https://github.com/user-attachments/assets/3b90a3dd-7d66-4d53-8b9d-60259cd7ad16" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

