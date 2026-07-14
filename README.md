# Alcohol-Consumption-Prediction-using-Machine-Learning

A binary classification project that predicts whether an individual
consumes alcohol using demographic, physical, and health-related attributes.

## Project Overview

The project compares multiple machine learning classification algorithms
for predicting alcohol-consumption status. It also examines the effect of
Principal Component Analysis (PCA) and repeated resampling on model performance.

## Dataset

The dataset contains 3,349 records and 24 columns:

- 23 input features
- 1 binary target variable: `DRK_YN`

The input features include:

- Age, sex, height, weight, and waistline
- Blood pressure and blood-sugar measurements
- Total, HDL, and LDL cholesterol
- Triglycerides and haemoglobin
- Liver-enzyme measurements
- Smoking status and other health indicators

No missing values were detected in the dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Methodology

1. Loaded and inspected the dataset
2. Checked for missing values
3. Encoded categorical variables
4. Separated the input features and target variable
5. Created an 80:20 train-test split
6. Trained four classification models
7. Evaluated the models using classification metrics
8. Applied PCA with six principal components
9. Performed repeated resampling to examine model stability

## Models Evaluated

- Perceptron
- Logistic Regression
- Support Vector Machine
- K-Nearest Neighbours

## Results

### Before PCA

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 72.2% |
| Perceptron | 70.6% |
| Support Vector Machine | 70.6% |
| K-Nearest Neighbours | 62.8% |

### After PCA

| Model | Test Accuracy |
|---|---:|
| Support Vector Machine | 62.7% |
| Logistic Regression | 61.0% |
| Perceptron | 59.1% |
| K-Nearest Neighbours | 57.6% |

Logistic Regression achieved the highest accuracy on the original fixed
test split. PCA reduced the dimensionality to six components but also
reduced model accuracy, indicating that the original features contained
important predictive information.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

## Running the Project

1. Clone this repository:

```bash
git clone https://github.com/Vishwateja-123/Alcohol-Consumption-Prediction-using-Machine-Learning.git
