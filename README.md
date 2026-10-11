# Customer Churn Prediction

## Project Overview
This project uses machine learning to predict customer churn for a telecommunications company. The objective is to identify customers who are likely to discontinue their services and help businesses improve customer retention.

## Dataset
- **Dataset:** IBM Telco Customer Churn
- **Original records:** 7,043
- **Records after cleaning:** 7,032
- **Features after encoding:** 30
- **Target variable:** Churn (Yes/No)

## Tools and Technologies
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow
1. Loaded and explored the dataset.
2. Analyzed churn distribution, tenure, and monthly charges.
3. Converted `TotalCharges` to numeric format.
4. Removed 11 records with missing `TotalCharges`.
5. Removed the customer ID column.
6. Encoded categorical variables.
7. Split the data into training and testing sets.
8. Trained three classification models.
9. Evaluated the models using accuracy, precision, recall, F1-score, and ROC-AUC.

## Model Performance

| Model | Accuracy | Churn Precision | Churn Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 80.4% | 64.8% | 57.5% | 60.9% | 0.836 |
| Balanced Logistic Regression | 72.6% | 49.1% | 79.7% | 60.8% | 0.835 |
| Random Forest | 76.8% | 55.5% | 65.2% | 60.0% | 0.821 |

## Key Findings
- Logistic Regression achieved the highest accuracy at 80.4%.
- Balanced Logistic Regression identified 79.7% of actual churners.
- Logistic Regression achieved the highest ROC-AUC score of 0.836.
- The choice of model depends on whether overall accuracy or identifying more potential churners is the business priority.

## Conclusion
The project demonstrates how machine learning can support customer retention by identifying customers at risk of leaving. The results highlight the trade-off between accuracy and churn recall. Further improvements could include hyperparameter tuning, threshold optimization, and testing additional classification algorithms.

## Skills Demonstrated
Python, data cleaning, exploratory data analysis, feature engineering, categorical encoding, classification, model evaluation, and data visualization.
