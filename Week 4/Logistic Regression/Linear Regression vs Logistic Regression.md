# Linear Regression vs Logistic Regression

## Linear Regression

Linear regression is commonly employed to predict continuous values. To illustrate its functionality, let's consider a scenario where we aim to predict the income of customers based on their age. By fitting a line or polynomial through the dataset, we can establish a mathematical equation to predict the income of a new customer given their age. However, linear regression is inadequate for predicting categorical variables such as churn.

## Logistic Regression

Unlike linear regression, logistic regression addresses the challenge of binary classification problems, such as churn prediction. By mapping the class labels to integer values (e.g., 0 and 1), logistic regression models the probability of class membership for each customer.

### The Sigmoid Function

Logistic regression employs a special function called the sigmoid function (or logistic function). This function outputs values between 0 and 1, representing the probability of an input belonging to a particular class. As the input value of the sigmoid function increases, the output approaches 1, indicating a higher probability of class membership.

### Training Process

To train a logistic regression model, we initialize the parameter vector and iterate through the following steps:

1. Calculate the model output using the sigmoid function.
2. Compare the predicted output with the actual label to determine the model's error.
3. Calculate the total error (cost) for all customers using the cost function.
4. Adjust the parameter values to minimize the cost through techniques like gradient descent.
5. Repeat the steps above until the cost is minimized, indicating an accurate model.

## Conclusion

Linear regression is suitable for predicting continuous values, while logistic regression is well-suited for binary classification problems. By leveraging the sigmoid function, logistic regression provides a probabilistic estimate of class membership, making it a valuable tool for predicting categorical variables.
