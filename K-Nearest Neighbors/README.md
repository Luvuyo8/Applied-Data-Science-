### **Project Overview: K-Nearest Neighbors**

#### **Objectives**
- Using the K-Nearest Neighbors (KNN) algorithm.
- Use KNN to classify customer data based on predefined categories.
- Optimize the K value to improve model accuracy.

---

#### **Introduction**
This project aims to explore the **K-Nearest Neighbors (KNN)** algorithm, a supervised machine learning technique used for classification and regression tasks. KNN predicts the class of a data point based on the classes of its nearest neighbors in the feature space. The algorithm determines the predicted class by majority voting among the \( K \) nearest neighbors.

Through this project, we analyze a telecommunications customer dataset to predict customer group membership. This information helps companies customize services and target offers more effectively.

---

#### **Dataset Overview**
The dataset includes customer demographic data such as:
- **Features:** `region`, `tenure`, `age`, `marital`, `address`, `income`, `education`, `employment`, `retirement`, `gender`, and `residence`.
- **Target:** `custcat` (Customer Category), representing four groups:
  - 1: Basic Service
  - 2: E-Service
  - 3: Plus Service
  - 4: Total Service

The goal is to classify customers into these categories using demographic attributes.

---

#### **Steps in the Project**

1. **Data Normalization**
   - Standardize the feature set \( X \) to ensure uniform scaling of all attributes, a crucial step since KNN is distance-based.
  
2. **Train-Test Split**
   - Split the dataset into training (80%) and testing (20%) sets for better evaluation of out-of-sample accuracy.
   
3. **Model Training with KNN**
   - Train the KNN model with different values of \( K \) and evaluate the accuracy.
  
4. **Prediction and Accuracy Evaluation**
   - Predict customer categories for the test dataset and compare with actual labels.
  
5. **Optimizing \( K \)**
   - Evaluate the model's accuracy for varying values of \( K \) to find the optimal number of neighbors.
   
---

#### **Results**
- **Accuracy for \( K = 4 \):** Train Accuracy = 54.75%, Test Accuracy = 32%.
- **Accuracy for \( K = 6 \):** Train Accuracy = 51.63%, Test Accuracy = 31%.
- **Optimal \( K = 9 \):** Achieved the highest test accuracy of 34%.

---

#### **Conclusion**
The project demonstrates the application of KNN to classify customer data effectively. The choice of \( K \) significantly impacts the model's performance, with \( K = 9 \) yielding the best results for this dataset. The insights gained can guide targeted marketing strategies and enhance customer satisfaction.
