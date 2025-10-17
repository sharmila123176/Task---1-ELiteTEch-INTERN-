# Task-1-ELiteTEch-INTERN
The goal is to classify or predict outcomes from a chosen dataset.
# THEORY: Building and Visualizing a Decision Tree Model Using Scikit-learn
# 1. Introduction
A Decision Tree is a supervised machine learning algorithm used for classification and regression tasks.
It works by splitting data into branches based on feature values, eventually reaching a decision at a leaf node.
For example, in a classification problem like predicting whether a flower is Iris Setosa or Iris Versicolor, the decision tree uses features such as petal length and petal width to make step-by-step decisions.
# 2. Objective of the Task
The main objective is to:
Build a Decision Tree model using the Scikit-learn library.
Train the model on a chosen dataset.
Visualize the tree structure to understand how the algorithm makes decisions.
Analyze the model’s performance using evaluation metrics such as accuracy, confusion matrix, and classification report.
# 3. Dataset Selection
The dataset used can be any labeled dataset suitable for classification or prediction.
Common choices include:
Iris Dataset – for classifying flower species.
Breast Cancer Dataset – for predicting malignant or benign tumors.
Titanic Dataset – for predicting survival of passengers.
Each dataset contains:
Features (X): Input variables (like age, petal length, income, etc.)
Target (y): The output or class label (like “Survived” or “Not Survived”).
# 4. Working Principle of Decision Trees
4.1 Concept
A Decision Tree divides the dataset into smaller and smaller subsets based on conditions on feature values.
It builds a tree-like structure with:
Root Node: The starting point of the tree representing the entire dataset.
Decision Nodes: Points where the data is split based on a feature.
Leaf Nodes: Final outcomes or predictions.
Example:

           [Petal length?]
               /       \
         <=2.45         >2.45
        Setosa      [Petal width?]
                         /     \
                     <=1.75     >1.75
                 Versicolor   Virginica

4.2 How the Tree Splits
The algorithm chooses the best feature to split the data at each step.
It uses mathematical criteria such as:
Gini Impurity: Measures how mixed the classes are at a node.
Entropy / Information Gain: Measures the reduction in uncertainty after a split.
The feature giving the highest information gain (or lowest impurity) becomes the decision node.
# 5. Steps in Building a Decision Tree Model
Step 1: Data Preprocessing
The dataset is cleaned and divided into:
Training set – to train the model.
Testing set – to evaluate its performance.
Step 2: Model Training
The model is built using the DecisionTreeClassifier() from Scikit-learn.
It learns patterns from the training data and stores them in the tree structure.
Step 3: Prediction
After training, the model predicts outcomes on new, unseen data using learned decision rules.
Step 4: Evaluation
Model performance is measured using:
Accuracy: Ratio of correct predictions to total predictions.
Confusion Matrix: Table showing true vs predicted classifications.
Classification Report: Displays precision, recall, and F1-score.
# Step 5: Visualization
Scikit-learn allows visualization of the decision tree using plot_tree() or export_graphviz().
