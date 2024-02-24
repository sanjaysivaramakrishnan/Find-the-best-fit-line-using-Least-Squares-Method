# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Sanjay sivaramakrishnan M
RegisterNumber:  212223240151

import numpy as np
import matplotlib.pyplot as plt
x = np.array([1,2,3,4,5,6,7,8,9,10])
y = np.array([11,12,13,14,15,16,17,18,19,20])
xmean = np.mean(x)
ymean = np.mean(y)
num = 0
den = 0 
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m = num/den
b = ymean-m*(xmean)
ypredicted = m*x-b
print("X-Vales: ",x)
print("y-Vales: ",y)
print("slope: ",m,", Intercept: ",b)
print("Y  predicted values: ",ypredicted)
plt.scatter(x,y)
plt.plot(x,ypredicted,color="green")
plt.show()
*/
```

## Output:
![Screenshot 2024-02-24 091015](https://github.com/sanjaysivaramakrishnan/Find-the-best-fit-line-using-Least-Squares-Method/assets/151629616/095a9571-a2c0-4886-aab1-66fce75183d8)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
