# Statistic Model

## Linear Regression

**Regression History**: Phenomenon regression, "A father's son height tends to regress the mean height", not tends to father's height.

**Concept**: Minimize the vertical distance between all the data points and out line.

**How**: sum of square errors, sum of absolute errors, least squares

* Residual: different between observed value and predicted value (observed - predicted), represent as *r*. It take Residual square (*r2*) because we don't need value to be negative, can't use absolute cause it'll give wrong result.
* bias (*b*): represent slope of linear.
* Least Squares: sum of squares residuals.
* Mean Square Error (MSE): residuals

## Logistic Regression

Logistic Regression is non-linear seperable data, classification.

Sigmoid Function: minimize output scale to 0-1 and make decision as 1: if >= 0.5, 0: if < 0.5