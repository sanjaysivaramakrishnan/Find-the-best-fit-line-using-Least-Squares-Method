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
#Input array -X and Y
X = np.array(eval(input()))
y = np.array(eval(input()))
print(X)
print(y)
# Mean Extraction
x_mean = np.mean(X)
y_mean = np.mean(y)
print(x_mean)
print(y_mean)
# num, denom = 0,0
#                                                  # using Normal python
# for i in range(len(X)):
#     num+= ((X[i]-x_mean) * (y[i] - y_mean))
#     denom += (X[i] - x_mean) **2
# m = num/denom
# b = y_mean - m*x_mean    
# print(m)
# print(b)
m = np.sum((X-x_mean)*(y-y_mean))/np.sum((X-x_mean)**2)
print(m)
b = y_mean - m*x_mean
print(b)
y_predicted = m*X + b
### Ploting
plt.scatter(X,y,color='#1df50a')
plt.xlabel('X Value')
plt.ylabel('Y Predicted')
_=plt.plot(X,y_predicted,color='#f24724')
y  = m*10 +b
print(y)
*/
```

## Output:
![image](https://github.com/user-attachments/assets/f3e23240-d155-44ff-83a9-989c535993f4)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
