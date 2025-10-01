# Bank Marketing Prediction with Random Forest

   This project applies a Random Forest classifier to the UCI Bank Marketing dataset, predicting whether a client will subscribe to a term deposit based on    demographic and campaign features.

# Project Objectives

  - Load and preprocess ~45,000 client records from the UCI Bank Marketing dataset.
  - Train and evaluate a Random Forest classifier for subscription prediction.
  - Analyze feature importances to identify key drivers of customer behavior.
  - Provide actionable insights for targeted marketing campaigns.
# Technologies Used

  - Python: pandas, NumPy, scikit-learn, matplotlib, seaborn
  - Machine Learning: Random Forest Classifier
  - Evaluation: accuracy, confusion matrix, precision/recall/F1

# what I did in code

   - Data Preprocessing
        Handled categorical features (job, contact, poutcome, etc.).
        Encoded months/days into numeric values.
        Split dataset into training, validation, and test sets.

    - Model Training
        Fit a Random Forest Classifier with tuned hyperparameters.
        Compared train/validation/test accuracy.
      
    - Evaluation
      Generated classification report with precision, recall, F1.
      Built confusion matrix to analyze prediction errors.
      
    - Interpretation
      Extracted feature importances (top drivers: balance, age, day, campaign).
      Visualized decision tree paths for interpretability.
    
