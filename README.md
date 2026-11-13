# Logistic Regression Optimizers

## Project Overview
This project implements and explores different optimization algorithms for Logistic Regression using the Titanic dataset.

The main goal is to understand how different optimizers affect model training, convergence, and classification performance.

## Dataset
- **Dataset:** Titanic Dataset
- **Source:** Kaggle
- **Number of Samples:** 891
- **Target Variable:** Survived

## Implemented Optimization Algorithms

1. Gradient Descent (GD)
2. Stochastic Gradient Descent (SGD)
3. Mini-Batch Gradient Descent
4. RMSProp
5. Adam

## Data Preprocessing
- Removed unnecessary columns.
- Handled missing values.
- Encoded categorical variables.
- Split the dataset into training and testing sets.
- Applied feature scaling using StandardScaler.

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## Tools and Libraries
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Best Result
Among the recorded results, **Stochastic Gradient Descent (SGD)** achieved the highest Accuracy of approximately **81.01%**.

## Conclusion
This project demonstrates the implementation of five optimization algorithms for Logistic Regression and explores their impact on model performance and training behavior.

The results show that SGD achieved the highest recorded Accuracy among the evaluated algorithms.

