# bank-marketing-rf



# Random Forest Bank Marketing Prediction

This repository contains a Jupyter Notebook (`random_forest_bank.ipynb`) demonstrating how to train and evaluate a Random Forest classifier on a bank marketing dataset. The goal is to predict whether a client will subscribe to a term deposit based on their demographic and transactional information.

## Table of Contents

- [Dataset](#dataset)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Visualization](#visualization)
- [Model Interpretation](#model-interpretation)


## Dataset

The dataset is derived from the Bank Marketing dataset provided by the UCI Machine Learning Repository. It includes information about clients contacted during marketing campaigns and whether they subscribed to a term deposit.

- **Source:** UCI Machine Learning Repository - Bank Marketing
- **Format:** CSV
- **Size:** ~45,000 records

## Features

The top features used by the Random Forest model (by importance) include:

1. `balance` (numeric): Average yearly balance in euros
2. `age` (numeric): Age of the client
3. `day` (numeric): Last contact day of the month
4. `month` (categorical→numeric): Last contact month
5. `job` (categorical): Type of job
6. `campaign` (numeric): Number of contacts performed during this campaign
7. `pdays` (numeric): Days since last contact
8. `contact` (categorical): Contact communication type
9. `poutcome` (categorical): Outcome of the previous marketing campaign
10. `housing` (binary): Has housing loan?

`

## Usage

1. Launch Jupyter Notebook:
   ```bash
jupyter notebook
```
2. Open `random_forest_bank.ipynb`.
3. Run the notebook cells in order to:
   - Load and preprocess the data
   - Split into training and test sets
   - Train a Random Forest classifier
   - Evaluate performance (accuracy, confusion matrix)
   - Visualize feature importances and distributions
   - Interpret the decision tree structure

## Results

After training the model, you should observe:

- **Accuracy** on the test set: ~0.74
- **Classification Report** on the test set:

  | Class | Precision | Recall | F1-score | Support |
  |-------|-----------|--------|----------|---------|
  | no    | 0.72      | 0.83   | 0.77     | 878     |
  | yes   | 0.77      | 0.64   | 0.70     | 797     |
  | **accuracy** |           |        | **0.74** | 1675    |
  | **macro avg** | 0.74      | 0.73   | 0.73     | 1675    |
  | **weighted avg** | 0.74      | 0.74   | 0.73     | 1675    |

- **Model Scores:**
  - Training set accuracy: `rfc.score(x_train, y_train)`
  - Validation set accuracy: `rfc.score(x_val, y_val)`
  - Test set accuracy: `rfc.score(x_test, y_test)`

## Visualization

The notebook provides plots for:

- Distribution of key numeric features (`age`, `balance`, `day`)
- Feature importance ranking
- Decision tree excerpt illustrating splits based on top features

## Model Interpretation

- **Feature Importances:** Identify which client attributes drive subscription likelihood.
- **Tree Visualization:** Understand specific decision rules (e.g., low `pdays` and high `balance` lead to higher subscription).

