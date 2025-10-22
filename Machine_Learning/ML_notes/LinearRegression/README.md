Linear Regression — Machine Learning Notes
 Overview

Linear Regression is a statistical method used to model the relationship between a dependent (target) variable and one or more independent (input) variables by fitting a linear equation to observed data.

It aims to find the best fit line that minimizes the difference between predicted and actual values.


`y_hat = m * x + c`



Where:

^𝑦 → Predicted output (target)

x → Input (feature)

m → Slope (weight)

c → Intercept (bias)


 Example

To predict the price of a home based on its area:

Price	Area
100	10
200	20
300	30

The data points approximately form a straight line. The best fit line can be used to predict prices for new areas.

⚙️ Mean Squared Error (MSE)

To find the best-fit line, we minimize the Mean Squared Error (MSE):


`MSE = (1/n) * Σ (y - y_hat)^2`


🔻 Cost Function / Loss Function

The loss function (L) measures the model error:

(`MSE = (1/n) * Σ (y - y_hat)^2`)



We apply Gradient Descent to minimize this loss and find the optimal 
𝑚 and 𝑐


🔽 Gradient Descent Update Rules

`𝑚_𝑛𝑒𝑤 = 𝑚_𝑜𝑙𝑑 − 𝛼(∂𝐿/∂𝑚)`


` c_new = c_old - 𝛼(∂𝐿/∂𝑐)`

	

Where:

α = learning rate

∂L/∂c = partial derivatives (gradients)

The algorithm iteratively updates 𝑚 and c until the loss reaches its minimum.

 Visualization

The minimum point of the loss function curve represents the best m and 𝑐 values.

At this point:

y_hat = mx + c

becomes the best-fit line.

Advantages

---Simple and easy to understand

---Works well for linear relationships

---Computationally efficient

---Good baseline model for regression tasks

---Provides feature importance

⚠️ Disadvantages

---Works only for linear relationships

---Sensitive to outliers

---Assumes linearity and independence of variables

---Can overfit with many features

---Not suitable for complex nonlinear patterns

🧾 Handwritten Notes

You can also view my original handwritten notes here:

📄 Linear Regression(1).jpeg

📄 Linear Regression(2).jpeg

📄 Linear Regression(3).jpeg

Summary

Linear Regression forms the foundation of many ML algorithms.
It teaches:

--how models learn relationships,

--how to optimize using loss functions, and

--how to interpret coefficients in a predictive model.


