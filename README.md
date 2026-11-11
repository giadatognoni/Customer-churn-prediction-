
# Customer Churn Prediction

## Project Overview

This project focuses on Customer Churn Prediction in the telecommunications industry.

The main objective is to analyze customer data and develop a Machine Learning model capable of identifying customers who are more likely to leave the service.

The project aims to support business decision-making by identifying potential churn risks and suggesting customer retention strategies.

## Dataset

The project uses the **Telco Customer Churn dataset**, which contains information about telecommunications customers.

- **Rows:** 7,043 customers
- **Columns:** 21 variables
- **Target variable:** `Churn`
- **Churn distribution:**
  - No: 5,174 customers (73.46%)
  - Yes: 1,869 customers (26.54%)

The dataset includes demographic information, services subscribed to, contract characteristics and customer charges.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Project Workflow

The project follows these main steps:

1. **Data Exploration (EDA):** analysis of the dataset structure, variables and customer churn distribution.
2. **Data Cleaning:** identification and management of missing values and data type conversion.
3. **Data Preprocessing:** numerical feature scaling, categorical feature encoding and missing value imputation using pipelines.
4. **Train-Test Split:** division of the dataset into training and test sets (80/20).
5. **Model Training:** development of two classification models:
   - Logistic Regression
   - Random Forest
6. **Model Evaluation:** comparison using Accuracy, Precision, Recall, F1-score and Confusion Matrix.
7. **Threshold Optimization:** evaluation of a 0.4 classification threshold to improve the identification of customers likely to churn.
8. **Business Insights:** interpretation of model results and development of customer retention recommendations.

## Model Performance

Logistic Regression achieved the best overall performance compared with Random Forest.

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 80.55% | 77.78% |
| Precision | 65.72% | 60.33% |
| Recall | 55.88% | 47.59% |
| F1-score | 60.40% | 53.21% |

Logistic Regression was selected as the reference model for further analysis.

### Classification Threshold Optimization

The default classification threshold of 0.5 was compared with a lower threshold of 0.4.

By reducing the threshold to 0.4:

- Recall increased from approximately 56% to 66%.
- More customers who actually churned were correctly identified.
- False positives increased.

This adjustment prioritizes the identification of potential churners, which can be particularly useful for customer retention activities.

## Key Business Insights

Exploratory Data Analysis revealed a strong association between contract type and customer churn.

| Contract Type | Churn Rate |
|---|---:|
| Month-to-month | 42.71% |
| One year | 11.27% |
| Two year | 2.83% |

Customers with monthly contracts show a significantly higher churn rate than customers with longer-term contracts.

### Business Recommendations

Based on these findings, the following strategies could help reduce customer churn:

- Offer discounts and promotions to encourage monthly customers to switch to annual or biennial contracts.
- Introduce personalized retention campaigns for customers identified as being at high risk of churn.
- Improve customer support and technical assistance.
- Monitor customer satisfaction and service quality.

A/B testing could also be used to evaluate the effectiveness of promotional campaigns.

## Model Limitations and Future Improvements

Although the model achieved promising results, it still has limitations, particularly in identifying all customers who actually churn.

Future improvements could include:

- Collecting additional information about internet connection problems.
- Analyzing technical support requests and home assistance interventions.
- Including activation and cancellation costs.
- Testing additional Machine Learning algorithms.
- Optimizing model hyperparameters.
- Evaluating model performance on new customer data.

## Conclusion

This project demonstrates how Machine Learning techniques can be applied to customer data to identify potential churn risks.

Beyond predictive modeling, the analysis highlights how data-driven insights can support business decisions and customer retention strategies.

The project represents a practical application of Python, data analysis and Machine Learning in a business context.

---

**Author:** Data Analysis Portfolio Project
:::
