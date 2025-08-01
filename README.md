

# Promotion Prediction Model - Machine Learning Project

## Project Overview

This project aims to predict employee promotions using various machine learning models. The goal is to accurately identify whether an employee will be promoted based on performance and demographic features.

## Dataset

The dataset contains employee details such as department, region, education, gender, recruitment channel, number of trainings, age, previous year rating, length of service, and KPI scores.

## Models Compared

* Logistic Regression (Base and Tuned)
* Random Forest (Base and Tuned)
* Extra Trees Classifier (Base and Tuned)
* XGBoost for even better results (XGBoost often handles imbalance well).

## Evaluation Metric

* The primary metric used for model evaluation is **F1 Score** on the positive class (promotion = 1), as this balances precision and recall and is critical for imbalanced classification.

## Results Summary

| Model                       | F1 Score (Class 1) | Precision (Class 1) | Recall (Class 1) | Accuracy |
| --------------------------- | ------------------ | ------------------- | ---------------- | -------- |
| Logistic Regression (Base)  | 0.29               | 0.18                | 0.70             | 0.705    |
| Logistic Regression (Tuned) | 0.28               | 0.17                | 0.75             | 0.680    |
| Random Forest (Base)        | **0.45**           | 0.44                | 0.47             | 0.905    |
| Random Forest (Tuned)       | 0.40               | 0.28                | 0.74             | 0.815    |
| Extra Trees (Base)          | **0.45**           | 0.42                | 0.48             | 0.900    |
| Extra Trees (Tuned)         | 0.44               | 0.38                | 0.52             | 0.890    |
|  XGBClassifier with  SMOTE  | 0.47               | 0.41                | 0.54             | 0.897    |
|  XGBClassifier without SMOTE| 0.51               | 0.87                | 0.36             | 0.941    |

## Conclusion

✅ If promotions are high-stakes and few → Use XGBoost without SMOTE 
✅ If you want to widen the promotion pool (e.g., training candidates) → Use XGBoost with SMOTE
## How to Use

1. Clone this repository.
2. Load the training and test datasets.
3. Run the provided scripts to preprocess the data and train the models.
4. Evaluate the models using the F1 score metric.
5. Use the selected model for predictions on new data.

## Dependencies

* Python 3.x
* pandas
* scikit-learn
* numpy

## Contact

For questions or feedback, please reach out to \[Your Name or Email].

---

If you want, I can also help you write a sample script or detailed instructions for running the code!
