# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

Step 1. import numpy as np

Step 2: from scipy package import lu

Step 3: get input from the user

Step 4: print result

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: VARUN JC
RegisterNumber: 212224240179
'''

import numpy as np
from scipy.linalg import lu
inp=eval(input())
A=np.array(inp,dtype=float)
P,L,U=lu(A)
print(L)
print(U) 
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: VARUN JC
RegisterNumber: 212224240179
'''

import numpy as np
from scipy.linalg import lu,solve_triangular
inp=eval(input())
inp1=eval(input())
A=np.array(inp,dtype=float)
B=np.array(inp1,dtype=float)
P,L,U=lu(A)
PB=P @ B
y = solve_triangular(L,PB,lower=True)
x = solve_triangular(U,y)
print(x)
*/
```

## Output:

<img width="1232" height="473" alt="image" src="https://github.com/user-attachments/assets/ec6b9fd0-7ce7-4bca-bff3-13dd4555c1cf" />

<img width="1234" height="263" alt="image" src="https://github.com/user-attachments/assets/02cd54a2-afb6-4738-8693-2fdce38af9f2" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

