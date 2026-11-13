# Logistic Regression Optimization Algorithms Comparison

## Project Overview

This project implements and compares different optimization algorithms used to train a Logistic Regression model.

The main goal is to understand how different optimization techniques affect the model's performance and to compare their results with and without Momentum.

The project uses the **Titanic dataset** to predict whether a passenger survived or not.

## Dataset

- **Dataset:** Titanic Dataset
- **Number of Rows:** 891
- **Number of Columns:** 12
- **Target Variable:** `Survived`

The target variable represents:
- `0`: Did not survive
- `1`: Survived

## Data Preprocessing

The following preprocessing steps were applied:

1. Loading the Titanic dataset.
2. Handling missing values.
3. Encoding categorical features:
   - Sex
   - Embarked
4. Separating the features (X) from the target variable (y).
5. Splitting the dataset into training and testing sets using an 80/20 ratio.
6. Applying StandardScaler to standardize the features.

The same dataset preparation approach was used across the experiments to ensure a fair comparison between optimization algorithms.

## Optimization Algorithms

The project compares the following five optimization algorithms:

1. Gradient Descent (GD)
2. Stochastic Gradient Descent (SGD)
3. Mini-Batch Gradient Descent
4. RMSProp
5. Adam

## Momentum

Momentum is used to improve optimization by considering previous updates when calculating the next parameter update.

In this project, Momentum was tested with:
- Gradient Descent
- Stochastic Gradient Descent
- Mini-Batch Gradient Descent
- RMSProp

A separate Adam with Momentum experiment was not implemented because Adam already incorporates momentum-based updates.

## Experimental Results

The models were evaluated using the following metrics:

- **Accuracy:** Measures the overall percentage of correct predictions.
- **Precision:** Measures how many predicted positive cases were actually positive.
- **Recall:** Measures how many actual positive cases were correctly identified.
- **F1 Score:** Represents the harmonic mean of Precision and Recall.
- **Confusion Matrix:** Shows the number of correct and incorrect predictions.

### Accuracy Comparison

| Optimization Algorithm | Without Momentum | With Momentum |
|---|---:|---:|
| Gradient Descent (GD) | 78.77% | 80.45% |
| Stochastic Gradient Descent (SGD) | 81.01% | 81.01% |
| Mini-Batch GD | 81.01% | 81.01% |
| RMSProp | 80.45% | 80.45% |
| Adam | 80.45% | N/A |

## Results Analysis

Based on the experimental results:

- **SGD and Mini-Batch GD** achieved the highest Accuracy of 81.01%.
- **Gradient Descent** improved from 78.77% to 80.45% after adding Momentum.
- **SGD** maintained the same Accuracy with and without Momentum.
- **Mini-Batch GD** maintained the same Accuracy in both experiments.
- **RMSProp** achieved 80.45% in both versions.
- **Adam** achieved an Accuracy of 80.45%.

Overall, SGD and Mini-Batch GD achieved the best Accuracy among the tested algorithms.

## Visualizations

The project includes visualizations to help understand and compare model performance, such as:

- Loss curves during training.
- Performance evaluation metrics.
- Confusion matrices.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Kaggle

## Conclusion

This project demonstrates how different optimization algorithms can affect Logistic Regression performance.

The experimental results show that SGD and Mini-Batch Gradient Descent achieved the highest Accuracy of 81.01%.

Adding Momentum improved the performance of Gradient Descent, while the Accuracy of SGD, Mini-Batch GD, and RMSProp remained unchanged.

The project provides a practical comparison of optimization algorithms and demonstrates the importance of selecting an appropriate optimization technique when training machine learning models.
