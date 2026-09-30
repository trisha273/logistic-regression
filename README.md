Logistic Regression 

📌 Project Overview

This project uses Machine Learning to predict whether a student will Pass or Fail based on different academic-related features.

In this project, Logistic Regression is implemented from scratch using NumPy. The model learns the relationship between student study-related features and the corresponding Pass/Fail outcome.

The goal of this project is to build a binary classification model that can predict whether a student is likely to pass or fail.

📌 Problem Statement

A student's academic performance can depend on several factors such as study hours and attendance.

In this project, two features are used to predict the student's result:

Hours Studied
Attendance Percentage

The model predicts whether the student will:

0 → Fail
1 → Pass

📌 Dataset

The dataset contains information about students along with their Pass/Fail outcomes.

The features used in this model are:

Hours Studied – Number of hours the student studied.
Attendance – Attendance percentage of the student.

The target variable is:

Student Result (Pass/Fail)

where:

0 = Fail
1 = Pass

The dataset contains 50 student records.

🛠️ Technologies Used

Python
Jupyter Notebook
NumPy
Matplotlib

📌 Machine Learning Model

This project implements Logistic Regression from scratch using Gradient Descent to predict whether a student will pass or fail.

The model learns the relationship between:

Input Features:

Hours Studied
Attendance

Target Variable:

Pass/Fail

The general workflow includes:

Creating and preparing the student dataset using NumPy.
Visualizing the relationship between student features and Pass/Fail results using Matplotlib.
Implementing the Sigmoid function to convert the model output into a probability.
Implementing a custom Cost Function to calculate the prediction error.
Implementing Gradient Calculation for the model parameters.
Implementing Gradient Descent from scratch to optimize the values of weights and bias.
Applying Feature Scaling to the input features.
Experimenting with different learning rates (alpha) and observing their effect on the final cost.
Plotting the Cost vs. Iterations graph.
Visualizing the Decision Boundary.
Making predictions using the trained Logistic Regression model.
Comparing predicted results with the actual Pass/Fail values.

The Logistic Regression model uses the sigmoid function to calculate the probability of a student passing.

The prediction is classified using a threshold:

Probability >= 0.5 → Pass
Probability < 0.5  → Fail

📈 Model Evaluation

The model is evaluated by calculating the cost function during the Gradient Descent process.

The cost measures the difference between the predicted probabilities and the actual Pass/Fail labels.

During training, Gradient Descent updates the values of the weights and bias to minimize the cost.

The project includes:

Initial cost calculation
Final cost calculation
Cost vs. Iterations graph
Learning rate comparison
Decision boundary visualization
Comparison between actual and predicted results
Accuracy calculation

The initial cost was approximately:

0.6811

After training, the final cost decreased to approximately:

0.1610

The model achieved an accuracy of approximately:

92%

A decreasing cost during training indicates that the model is learning and improving its predictions.

📚 Key Learnings

Through this project, I learned:

The fundamentals of Logistic Regression and how it can be used for binary classification.
How to implement Logistic Regression from scratch using NumPy.
How the Sigmoid function converts model output into probabilities.
How to calculate the Logistic Regression cost function.
How Gradient Descent updates model parameters to minimize the cost.
The importance of choosing an appropriate learning rate.
Why Feature Scaling is useful during model training.
How to visualize student data using Matplotlib.
How to plot and analyze Cost vs. Iterations.
How to visualize a Decision Boundary for classification.
How to compare actual and predicted results.
How to calculate the accuracy of a classification model.

🔮 Future Improvements

Possible improvements to this project include:

Using a larger and more realistic student performance dataset.
Adding more features such as previous exam scores, assignments, study habits, and sleep hours.
Using a larger training and testing dataset.
Splitting the dataset into training and testing sets to evaluate performance on unseen data.
Adding evaluation metrics such as Precision, Recall, F1-Score, and Confusion Matrix.
Comparing the custom Logistic Regression implementation with Scikit-learn's Logistic Regression.
Experimenting with different feature scaling techniques.
Improving the visualization of the decision boundary.
Testing different learning rates and numbers of iterations.
Trying other classification algorithms such as KNN, Decision Tree, Random Forest, and SVM.

👩‍💻 Author

Trisha Mallick

GitHub: github.com/trisha273
