Summary of Preprocessing Steps
Step	Action Taken	Reason
Missing Values	Checked (None found)	Prevents bias and model errors
Feature Scaling	StandardScaler applied	Ensures equal importance of all features

Classification Algorithms and Their Suitability for the Breast Cancer Dataset
1. Logistic Regression
✅ How It Works:

A statistical method used for binary classification (e.g., benign vs. malignant).

Uses the logistic (sigmoid) function to predict probabilities.

Decision threshold (default = 0.5) is applied to classify outputs as 0 (benign) or 1 (malignant).

✅ Why It’s Suitable?

Works well for linearly separable datasets.

Provides probabilistic interpretation of predictions.

Computationally efficient and robust to noise.

2. Decision Tree Classifier
✅ How It Works:

Splits the data based on feature values to create a tree-like structure.

Uses if-else rules to classify data points.

The model continues splitting until a stopping criterion is met (e.g., maximum depth).

✅ Why It’s Suitable?

Easy to interpret and visualize.

Works well with both linear and non-linear data.

Handles imbalanced datasets effectively.

However, prone to overfitting, which can affect accuracy.

3. Random Forest Classifier
✅ How It Works:

An ensemble of multiple decision trees.

Uses bagging (bootstrap aggregation) to create random subsets of data.

Final prediction is based on majority voting across trees.

✅ Why It’s Suitable?

Reduces overfitting compared to a single decision tree.

Performs well on high-dimensional datasets like this one.

Can handle missing values and noisy data effectively.

4. Support Vector Machine (SVM)
✅ How It Works:

Finds the optimal hyperplane that separates the two classes.

Uses kernel functions (linear, polynomial, RBF) to handle non-linear data.

Maximizes the margin between the two classes for better generalization.

✅ Why It’s Suitable?

Works well with high-dimensional data.

Effective in cases where the data is not linearly separable.

Robust against overfitting, especially with regularization.

5. k-Nearest Neighbors (k-NN)
✅ How It Works:

A lazy learning algorithm that doesn’t train a model explicitly.

When making a prediction, it finds the k closest data points in the training set.

Classifies the new data point based on majority voting of its neighbors.

✅ Why It’s Suitable?

Simple and non-parametric (no assumption about data distribution).

Works well when the decision boundary is non-linear.

However, computationally expensive for large datasets.

Summary Table
Algorithm	How It Works	Why It’s Suitable for Breast Cancer Dataset
Logistic Regression	Uses sigmoid function for binary classification	Works well for linearly separable data, interpretable
Decision Tree	Splits data based on features into a tree structure	Handles both linear and non-linear relationships but prone to overfitting
Random Forest	Uses multiple decision trees and majority voting	Reduces overfitting, handles high-dimensional data
SVM	Finds optimal hyperplane for classification	Works well for complex, high-dimensional datasets
k-NN	Classifies based on nearest neighbors	Good for non-linear
