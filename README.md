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

    -  Model Training
        Fit a Random Forest Classifier with tuned hyperparameters.
        Compared train/validation/test accuracy.

# Impact & Applications

  - Banking & Finance: optimize marketing campaigns, reduce call costs, target high-probability clients.
   - Business Intelligence: combine ML predictions with customer profiling.
   - Cross-domain: methods can generalize to churn prediction, fraud detection, or loan default risk.

  #   Research Extensions 

   - Compare Random Forest with XGBoost/LightGBM for improved accuracy.
   - Apply SHAP/LIME for deeper interpretability.
   - Explore fairness metrics (are predictions biased by age or job type?).
    - Extend to time-aware models to incorporate campaign history.

   
        
      
    -  Evaluation
      Generated classification report with precision, recall, F1.
      Built confusion matrix to analyze prediction errors.
      
    -  Interpretation
      Extracted feature importances (top drivers: balance, age, day, campaign).
      Visualized decision tree paths for interpretability.

  # Results

   - Test Accuracy: 0.74
    - Precision / Recall / F1:
    
- Class	Precision Recall F1-score Support
- no	0.72	0.83	0.77	878
- yes	0.77	0.64	0.70	797
- Overall	–	–	0.74	1,675

    - Feature Importances (top 3):

       Balance (avg yearly account balance)
        Age
       Number of contacts in campaign

- Insight: Customers with higher balances, contacted after fewer days (pdays), and in fewer overall campaign calls were most likely to subscribe.

  # Visual Examples

- Distribution of customer ages and balances.
- Elbow curve of feature importances.
- Decision tree excerpt showing rule splits.
  
    
