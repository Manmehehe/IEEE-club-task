Section 1:
1. logistic regression model
2.

def fibonacci(n):
    # Initialize the first two terms
    a, b = 0, 1
    terms = []
    
    for _ in range(n):
        terms.append(a)
        # Update the values for the next iteration
        a, b = b, a + b
        
    return terms

# Get user input
n = int(input("Enter the number of terms to generate in the Fibonacci sequence: "))
fibonacci_terms = fibonacci(n)

# Print the Fibonacci sequence
print("The first", n, "terms of the Fibonacci sequence are:")
print(fibonacci_terms)



3. queue
4. varialble_1
5. merge sort

https://docs.google.com/document/d/1Sgv_v8e4OWg40b1g66TVyBYFQFm_6_QAIHsIJsi1ZA0/edit?usp=sharing (this is a google dox file of my tasks including poster and summary of the research paper)


This code implements a basic linear regression model from scratch using Python, without relying on machine learning libraries like scikit-learn. The goal is to predict salaries based on years of experience using gradient descent for optimization. Here's a breakdown of the approach:

Class: LinearRegressionBasic
Initialization (__init__):

learning_rate: Controls the step size during gradient descent.
n_iterations: The number of times the gradient descent optimization process is repeated.
m: The slope of the line (initially set to 0).
b: The y-intercept of the line (initially set to 0).
Model Training (fit method):

Takes two inputs: X (years of experience) and Y (salaries).
Uses gradient descent to minimize the error between predicted and actual salaries by adjusting m (slope) and b (intercept).
For each data point, the gradients (dm for slope and db for intercept) are calculated based on the error between the predicted and actual salary.
The model updates m and b iteratively, adjusting them to minimize the overall prediction error.
Prediction (predict method):

Takes a list of input values (X) and applies the learned linear equation y = mx + b to make predictions.
Returns the predicted salary for each input.
User Input and Model Execution
get_user_input():
A function that prompts the user to enter data points (years of experience and corresponding salaries) for several employees, which are used for training the model.

Main Execution:

Takes user input for the years of experience and salaries.
Initializes the model, trains it using the fit method, and makes salary predictions.
Optionally, the user can enter a new number of years of experience, and the model predicts the corresponding salary.
Key Concepts:
Gradient Descent: Used to iteratively update the slope and intercept to minimize the prediction error.
Linear Equation: The model predicts salary using the linear equation y = mx + b based on the learned parameters m and b.
Advantages:
Simple implementation using basic Python operations.
Demonstrates how linear regression works without relying on external machine learning libraries.
This approach is ideal for learning how linear regression and gradient descent function at a fundamental level.
