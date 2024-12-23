# Logistic Regression from Scratch

This project implements logistic regression from scratch using Python and NumPy. The goal is to classify kidney stone cases using the "Kidney Stone Urine Analysis" dataset. The implementation includes regularization and evaluates the model's performance on validation and test datasets.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Implementation Steps](#implementation-steps)
4. [Performance](#performance)
5. [How to Run](#how-to-run)
6. [Future Improvements](#future-improvements)

---

## Project Overview

Logistic regression is a fundamental machine learning algorithm used for binary classification. In this project:

- Logistic regression is implemented from scratch without using libraries like `scikit-learn`.
- The dataset is split into training, validation, and test sets.
- Regularization is added to prevent overfitting.
- The model is evaluated using metrics like accuracy.

---

## Dataset Description

The dataset used in this project, `kindeyStoneUrineAnalysis.csv`, contains the following features:

- **Independent Variables**: `gravity`, `ph`, `osmo`, `cond`, `urea`, `calc`
- **Target Variable**: `target` (binary classification)

The data is preprocessed to handle:

- Missing values (none found in this dataset).
- Feature scaling using standardization (z-score normalization).

---

## Implementation Steps

1. **Exploratory Data Analysis (EDA)**:

   - Checked for categorical and numerical data.
   - Verified the absence of missing values.

2. **Data Splitting**:

   - Training set: 80%
   - Validation set: 10%
   - Test set: 10%

3. **Standardization**:

   - Standardized features to have zero mean and unit variance.

4. **Logistic Regression Implementation**:

   - Forward propagation (linear transformation and sigmoid function).
   - Cost function (binary cross-entropy loss).
   - Gradient descent optimization for weights and biases.
   - Regularization to penalize large weights.

5. **Evaluation**:

   - Validated the model on both validation and test datasets.

---

## Performance

The model achieved the following accuracy:

- **Validation Accuracy**: 62.5%
- **Test Accuracy**: 75.0%

---

## How to Run

### Prerequisites

- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

### Steps

1. Clone or download this repository.
2. Ensure the dataset `kindeyStoneUrineAnalysis.csv` is in the `DataSet/` directory.
3. Run the script `logistic_regression_from_scratch.py`.
4. Observe the cost reduction and accuracy on validation and test datasets.

---

## Future Improvements

1. **Hyperparameter Tuning**:

   - Experiment with different values for learning rate and regularization strength.

2. **Model Performance**:

   - Investigate why regularization does not improve validation accuracy significantly.
   - Analyze the impact of dataset size and feature importance.

3. **Feature Engineering**:

   - Explore additional transformations or derived features to improve model accuracy.

---

This project serves as a foundational implementation to understand the workings of logistic regression and regularization. Contributions and feedback are welcome!

