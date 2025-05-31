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

Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: 212224220062
RegisterNumber: Meenakshi.R

/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Lathika K
RegisterNumber:212224230140

import numpy as np
import matplotlib.pyplot as plt
x = np.array(eval(input("Enter X values as a list: ")))
y = np.array(eval(input("Enter Y values as a list: ")))

x_mean = np.mean(x)
y_mean = np.mean(y)

num = np.sum((x - x_mean) * (y - y_mean))
denom = np.sum((x - x_mean) ** 2)

m = num / denom
b = y_mean - m * x_mean

print(f"Slope (m): {m}")
print(f"Y-Intercept (b): {b}")

y_predicted = m * x + b
print("Predicted Y values:", y_predicted)

plt.scatter(x, y, label="Actual Data", color="blue")
plt.plot(x, y_predicted, color="red", label="Regression Line")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.legend()
plt.title("Linear Regression")
plt.show()
*/

## Output:


![Screenshot (124)](https://github.com/user-attachments/assets/7a7e8fbe-2c49-4e98-85b1-633e5c645c08)

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
