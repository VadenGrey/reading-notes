# Class 13

**How to Run Linear Regression in Python**

Linear regression can be thought of as finding the straight line that best fits a set of scattered data points.

How to Create a Linear Regression and Display it:
```python
# Import the packages and classes needed for this example:
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Create random data with numpy, and plot it with matplotlib:
rnstate = np.random.RandomState(1)
x = 10 * rnstate.rand(50)
y = 2 * x - 5 + rnstate.randn(50)
plt.scatter(x, y);
plt.show()

# Create a linear regression model based the positioning of the data and Intercept, and predict a Best Fit:
model = LinearRegression(fit_intercept=True)
model.fit(x[:, np.newaxis], y)
xfit = np.linspace(0, 10, 1000)
yfit = model.predict(xfit[:, np.newaxis])

# Plot the estimated linear regression line with matplotlib:
plt.scatter(x, y)
plt.plot(xfit, yfit);
plt.show()
```

**Linear Regression in Python**

Regression analysis explores the relationship between a quantitative response variable and one or more explanatory variables.

If there's only one explanatory variable its called simple linear regression, if there's more than one then its multiple regression

references

[How to Run Linear Regression in Python](https://www.activestate.com/resources/quick-reads/how-to-run-linear-regressions-in-python-scikit-learn/)

[Linear Regression in Python](https://www.youtube.com/watch?v=KsVBBJRb9TE&ab_channel=jbstatistics)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)