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
