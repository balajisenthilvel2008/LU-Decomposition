# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Problem 1
  1. Import the numpy and scipy.linalg module to use the built-in functions for calculation like lu()
  2. Get the input using eval(input()) and convert it into a matrix using np.array()
  3. Find the L and U matrix using lu()
  4. Print the values and end the program
### Problem 2
  1. Import the numpy and scipy.linalg module to use the built-in functions for calculation like lu_factor(), lu_solve()
  2. Get the input using eval(input()) and convert it into a matrix using np.array()
  3. Decompose the matrix using lu_factor() and solve the matrix using lu_solve()
  4. Print the values and end the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: BALAJI S
RegisterNumber: 25012884
'''
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: BALAJI S
RegisterNumber: 25012884
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
```

## Output:
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/936cdae1-bcc6-4cba-890b-f3a85b196855" />

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/db32c409-9d9b-4bbc-8b89-29edb71bf109" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

