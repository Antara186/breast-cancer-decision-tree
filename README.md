**Dataset**

This project uses the Breast Cancer Wisconsin Dataset, which is built into the scikit-learn library.

The dataset is loaded using:

from sklearn.datasets import load_breast_cancer


data = load_breast_cancer()
Dataset Information
Total samples: 569
Total features: 30
Training samples: 426
Testing samples: 143
Problem type: Binary Classification
Target Classes

The dataset contains two classes:

Malignant
Benign

The objective is to build a machine learning model that can classify breast tumors based on their measured features.

**Objectives**

The main objectives of this project are:

To analyze the Breast Cancer Wisconsin Dataset.
To preprocess and prepare the dataset for machine learning.
To select the most important features using SelectKBest.
To build a Decision Tree classification model.
To analyze overfitting in an unregularized Decision Tree.
To apply regularization techniques to improve model generalization.
To optimize Decision Tree hyperparameters using GridSearchCV.
To perform hyperparameter optimization using RandomizedSearchCV.
To explore Bayesian optimization using Optuna.
To evaluate and compare the performance of different models.

## Technologies Used

- **Python** — Programming language
- **NumPy** — Numerical computation
- **Pandas** — Data manipulation and analysis
- **Matplotlib** — Data visualization
- **Scikit-learn** — Machine learning and model evaluation
- **Optuna** — Hyperparameter optimization
- **Jupyter Notebook** — Development and experimentation

**  Methodology**

The project follows these steps:

Load the Dataset
Load the Breast Cancer Wisconsin Dataset using scikit-learn.
Data Preparation
Separate the input features (X) and target variable (y).
Split the dataset into training and testing sets.
Feature Selection
Use SelectKBest with the ANOVA F-test to select the top 10 features.
Decision Tree Classification
Train an initial unregularized Decision Tree classifier.
Evaluate its training and testing performance.
Overfitting Analysis
Compare training and testing accuracy to identify potential overfitting.
Decision Tree Regularization
Apply parameters such as max_depth, min_samples_split, and min_samples_leaf to control tree complexity.
Hyperparameter Optimization
Use GridSearchCV to find suitable hyperparameters.
Use RandomizedSearchCV for randomized hyperparameter search.
Use Optuna for Bayesian hyperparameter optimization.
Model Evaluation
Compare the performance of the different Decision Tree models using appropriate evaluation metrics.

**Results**

The project evaluates multiple Decision Tree models and compares their performance using training accuracy, testing accuracy, and cross-validation.

Models Evaluated
Unregularized Decision Tree
Regularized Decision Tree
Grid Search Decision Tree
Random Search Decision Tree
Optuna Decision Tree
Evaluation Metrics

The models are evaluated using:

Training Accuracy
Testing Accuracy
Confusion Matrix
Classification Report
Cross-Validation Mean Accuracy
Cross-Validation Standard Deviation
Model Comparison

The performance of the different Decision Tree models is compared based on their training accuracy, testing accuracy, tree depth, and number of leaves.

The models are ranked according to their testing accuracy to identify the best-performing model.

Cross-Validation

5-fold cross-validation is performed to evaluate the stability and generalization performance of the models.

The mean cross-validation accuracy and standard deviation are calculated for each model.

Overfitting Analysis

The unregularized Decision Tree is compared with the regularized Decision Tree to analyze overfitting and model complexity.

Regularization is applied using:

max_depth = 4
min_samples_leaf = 5
min_samples_split = 10
Hyperparameter Optimization

Three hyperparameter optimization approaches are explored:

GridSearchCV
RandomizedSearchCV
Optuna

These methods are used to search for better Decision Tree hyperparameter configurations and improve model performance.

Visualizations

The project also includes:

Confusion Matrix
Classification Report
Decision Tree Visualization
Decision Boundary Visualization
Model Performance Comparison

**Conclusion**

This project demonstrates the application of Decision Tree classification to the Breast Cancer Wisconsin Dataset.

Feature selection using SelectKBest was used to identify important features before model training. Different Decision Tree configurations were investigated, including unregularized and regularized models.

Hyperparameter optimization was performed using GridSearchCV, RandomizedSearchCV, and Optuna. The models were evaluated using testing accuracy and cross-validation to compare their performance and generalization.

Overall, the project provides a complete machine learning workflow covering data preparation, feature selection, model development, regularization, hyperparameter optimization, evaluation, and visualization.
