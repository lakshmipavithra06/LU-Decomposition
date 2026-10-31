# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## i) To find the L and U matrix

Step 1: Import numpy module and lu function from scipy.linalg.

Step 2: Get the matrix input from the user.

Step 3: Use lu() function to obtain P, L and U matrix.

Step 4: Print L and U matrix.

## (ii) To find the LU Decomposition of a matrix

Step 1: Import numpy module and lu_factor() and lu_solve() functions from scipy.linalg.

Step 2: Get the input matrices A and B from the user.

Step 3: Use lu_factor() to get L and U and use lu_solve() to get the solution vector X.

Step 4: Print the solution vector X. 

## Program:
## (i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: LAKSHMI PAVITHRA M
RegisterNumber:212225220055 
'''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
## (ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: LAKSHMI PAVITHRA M
RegisterNumber: 212225220055
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)


```

## Output:
## (i)
<img width="1367" height="837" alt="image" src="https://github.com/user-attachments/assets/b89a933f-5d44-460b-b60b-559d075ed10b" />

<img width="1505" height="560" alt="image" src="https://github.com/user-attachments/assets/b7863b61-4398-4f8f-8738-8f505d33effe" />

## (ii)
<img width="1152" height="828" alt="image" src="https://github.com/user-attachments/assets/b92fbdee-4669-42a9-9c77-6da50f420f46" />

<img width="1291" height="260" alt="image" src="https://github.com/user-attachments/assets/a886047b-5382-4852-8ffb-8fefc27140d1" />






## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

