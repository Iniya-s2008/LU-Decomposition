# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Import the required libraries numpy and scipy.linalg.

Step 2: Define the input matrix A.

Step 3: Apply the lu() function to decompose matrix A into P, L, and U matrices.

Step 4: Display the lower triangular matrix L and upper triangular matrix U.

Step 5: Stop the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: INIYA S
RegisterNumber: 212225230104
*/
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: INIYA S
RegisterNumber: 212225230104
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
res=lu_solve((piv,lu),constant)
print(res)


```

## Output:
![lu decomposition]()
<img width="1247" height="845" alt="image" src="https://github.com/user-attachments/assets/443b7f1a-b262-4496-a244-e3000dc98a10" />
<img width="1227" height="762" alt="image" src="https://github.com/user-attachments/assets/a87b09a6-c7aa-43c3-8917-59a8b7d4a63e" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

