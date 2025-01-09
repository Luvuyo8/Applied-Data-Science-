### Project Overview: Logistic Regression with Python

#### Objectives
1. Use scikit-learn's Logistic Regression to classify.
2. Understand and interpret the confusion matrix.

#### Introduction
In this project, a model is created for a telecommunications company to predict customer churn. The goal is to identify customers likely to leave for a competitor and enable the company to take proactive measures to retain them. Customer retention is often more cost-effective than acquisition, making churn prediction crucial for maintaining a stable customer base.

---

### **Problem Description**
A telecommunications company is facing customer churn, especially in its landline business. As an analyst, the task is to identify which customers are leaving and understand the factors contributing to this behavior.

---

### **Dataset Information**
The dataset is a historical record, with each row representing a customer. Key information includes:
- **Churn Status**: Whether the customer left in the last month.
- **Services**: Subscriptions like phone, internet, streaming, etc.
- **Account Details**: Contract duration, payment methods, billing type, and charges.
- **Demographics**: Gender, age range, marital status, and dependents.

---

### **Steps in Analysis**

#### 1. **Data Preparation**
The "Telco Churn" dataset is loaded and explored. Each case corresponds to a unique customer with various features indicating their behavior, demographics, and account details.

#### 2. **Model Building**
The `LogisticRegression` function from Scikit-learn is used to train the model. Key details:
- Logistic regression supports regularization to prevent overfitting.
- Different solvers like ‘newton-cg’, ‘lbfgs’, and ‘saga’ are available.

#### 3. **Evaluation Metrics**
- **Jaccard Index**: Measures the intersection divided by the union of the predicted and true label sets. For this model:  
  `jaccard_score(y_test, yhat, pos_label=0) = 0.753`
- **Confusion Matrix**: Provides a detailed breakdown of true positives, true negatives, false positives, and false negatives.  
  Example:
  - True Positives (TP): Correctly predicted churners.
  - False Positives (FP): Non-churners predicted as churners.
  - Accuracy: 0.78 (78% of predictions were correct).
  
- **Precision, Recall, and F1-Score**:
  ```
              Precision    Recall   F1-Score   Support
  Class 0      0.81       0.91       0.86      1035
  Class 1      0.63       0.42       0.50       374
  ```

- **Log Loss**: Measures model performance when outputs are probabilities. Lower values indicate better predictions.
  `log_loss(y_test, yhat_prob) = 0.471`

---

### **Insights from Evaluation**
- The model performs well in predicting non-churners (Class 0), achieving 91% recall.
- Churners (Class 1) are harder to predict, with a recall of 42%.
- The overall F1-Score is 0.76, reflecting balanced performance between precision and recall.

---

### **Conclusion**
The logistic regression model provides a reliable baseline for predicting customer churn. However, improvements can be made to better capture churners, such as:
- Incorporating additional features or using feature engineering.
- Exploring ensemble methods or advanced algorithms for comparison.

This analysis demonstrates the practical use of logistic regression for business insights and highlights the importance of evaluation metrics in assessing model performance.
