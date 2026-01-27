# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the linear regression using gradient descent.
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# -----------------------
# Load Data
# -----------------------
data = pd.read_csv("50_Startups.csv")

# Select input (X) and output (Y)
x = data["R&D Spend"].values
y = data["Profit"].values

# -----------------------
# Parameters
# -----------------------
w = 0.0
b = 0.0
alpha = 0.00000001   # Small learning rate
epochs = 100
n = len(x)

losses = []

# -----------------------
# Gradient Descent
# -----------------------
for _ in range(epochs):

    # Prediction
    y_hat = w * x + b

    # Mean Squared Error
    loss = np.mean((y_hat - y) ** 2)
    losses.append(loss)

    # Gradients
    dw = (2/n) * np.sum((y_hat - y) * x)
    db = (2/n) * np.sum(y_hat - y)

    # Update parameters
    w = w - alpha * dw
    b = b - alpha * db

# -----------------------
# Plot Results
# -----------------------
plt.figure(figsize=(12, 5))

# Loss vs Iterations
plt.subplot(1, 2, 1)
plt.plot(losses)
plt.xlabel("Iterations")
plt.ylabel("Loss (MSE)")
plt.title("Loss vs Iterations")

# Regression Line
plt.subplot(1, 2, 2)
plt.scatter(x, y)
plt.plot(x, w * x + b)
plt.xlabel("R&D Spend")
plt.ylabel("Profit")
plt.title("Linear Regression Fit")

plt.tight_layout()
plt.show()

print("Final weight (w):", w)
print("Final bias (b):", b)


Developed by: ALAPATI KRANTHI KIRAN
RegisterNumber:  212225230012
*/
```

## Output:
![linear regression using gradient descent](sam.png)
![alt text](<Screenshot 2026-01-27 091104.png>)

## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
