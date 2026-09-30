Logistic Regression 

📌 Project Overview

This project implements a Logistic Regression model from scratch using NumPy to predict whether a student will Pass or Fail based on:

Hours Studied
Attendance Percentage

Instead of using a ready-made machine learning library for Logistic Regression, the main parts of the algorithm are implemented manually, including the sigmoid function, cost function, gradient calculation, and gradient descent.

🎯 Objective

The objective of this project is to understand how Logistic Regression works internally and use it for a binary classification problem.

The model predicts:

0 → Fail
1 → Pass
📊 Dataset

The dataset contains 50 student records.

Each student has two features:

Feature       	      Description
Hours Studied	      Number of hours studied
Attendance	       Attendance percentage
Target	           Pass (1) or Fail (0)

The target variable is:

0 = Fail
1 = Pass

🛠️ Technologies Used
Python
NumPy
Matplotlib
Jupyter Notebook

🔄 Project Workflow

The project follows these steps:

Create the student dataset.
Visualize the Pass/Fail data.
Implement the sigmoid function.
Calculate the logistic regression cost.
Calculate gradients.
Implement gradient descent.
Apply feature scaling.
Train the model.
Compare different learning rates.
Plot the learning curve.
Plot the decision boundary.
Make predictions.
Calculate model accuracy.

🧠 Logistic Regression Implementation

1. Sigmoid Function

The sigmoid function converts the model's output into a probability between 0 and 1.

def sigmoid(z):
    g = 1 / (1 + np.exp(-z))
    return g
    
2. Cost Function

A logistic regression cost function is implemented to measure the model's error.

def compute_cost(x, y, w, b):

The initial cost in this project was approximately:

0.6811

After training, the final cost decreased to:

0.1610

3. Gradient Calculation

The gradients of the weights and bias are calculated manually using:

def compute_gradient(x, y, w, b):

4. Gradient Descent

Gradient descent is used to update the weights and bias and minimize the cost.

def compute_gradient_descent(x, y, w_in, b_in, alpha, iters):

The model uses:

Learning Rate (alpha) = 0.035
Iterations = 10,000

⚙️ Feature Scaling

Feature scaling is applied before training because the two input features have different ranges.

x_mean = np.mean(x_train, axis=0)
x_std = np.std(x_train, axis=0)

x_scaled = (x_train - x_mean) / x_std

This standardizes the features and helps gradient descent converge more effectively.

📈 Learning Rate Comparison

Different learning rates were tested:

Learning Rate	      Final Cost
0.015              	0.1642
0.020	              0.1632
0.025             	0.1624
0.030	              0.1617
0.035	              0.1610

The project uses 0.035 as the learning rate for the final model.

🔢 Trained Parameters

After training for 10,000 iterations:

w = [3.60237076, 1.86257304]

b = -0.7336224417

These parameters are used to calculate the probability of a student passing.

🎯 Prediction

The prediction function calculates the sigmoid probability and applies a threshold of 0.5.

Probability >= 0.5 → Pass (1)
Probability < 0.5  → Fail (0)

📊 Model Performance

The model achieved an accuracy of:

92.0%

The predictions were compared with the actual Pass/Fail labels to calculate the accuracy.

📉 Visualizations

The project includes the following visualizations:

1. Student Pass/Fail Data

A scatter plot showing students based on:

Hours studied
Attendance
2. Cost vs Iterations

A learning curve showing how the cost decreases during gradient descent.

3. Decision Boundary

A decision boundary separating the predicted Pass and Fail classes.

📂 Project Structure
Logistic-Regression/
│
├── logistic_regression(new)-checkpoint.ipynb
└── README.md

📚 Key Learnings

Through this project, I learned:

How Logistic Regression works internally.
How the sigmoid function is used for classification.
How to calculate logistic regression cost.
How gradients are calculated.
How gradient descent trains a model.
Why feature scaling is important.
How a decision boundary separates two classes.
How to evaluate classification accuracy.

👩‍💻 Author

Trisha Mallick
GitHub: (https://github.com/trisha273)
