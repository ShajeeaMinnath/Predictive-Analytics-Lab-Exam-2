# Predictive Analytics Lab Exam-2

## Objective
To perform classification using machine learning techniques and analyze model performance.

## Dataset
- Total entries: 1020
- Features: Feature1, Feature2
- Target: Binary classification (Yes/No)

## Exploratory Data Analysis (EDA)
- Found missing values in target column → removed using dropna()
- Detected extreme outliers in Feature1 → removed
- Visualized feature distribution using scatter plot
- Observed non-linear (circular) pattern in data

## Data Preprocessing
- Encoded target variable using LabelEncoder
- Scaled features using StandardScaler

## Model Building
- Initial model: Logistic Regression (linear)
- Issue: Poor performance due to non-linear data
- Final model: Polynomial Features + Logistic Regression using Pipeline

## Decision Boundary
- Linear model → straight line (poor fit)
- Polynomial model → curved boundary (correct fit)

## Model Evaluation
- Accuracy: 96%
- Confusion Matrix:
  [[151   8]
   [  0  41]]

- Classification Report:
  - High precision and recall
  - 100% recall for minority class

## Conclusion
Polynomial feature transformation successfully captured the non-linear pattern in the dataset, significantly improving classification performance.
