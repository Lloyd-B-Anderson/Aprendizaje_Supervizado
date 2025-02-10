# Customer Churn Prediction - Beta Bank

## Project Overview
Beta Bank has been experiencing customer churn, which directly impacts revenue and customer retention efforts. Since acquiring new customers is more costly than retaining existing ones, this project aims to build a predictive model that can identify potential churners. By leveraging machine learning, the goal is to optimize both the **F1-score** and **AUC-ROC**, ensuring an effective and balanced approach to churn prediction.

## Objectives
- Develop a machine learning model to predict customer churn with high accuracy.
- Achieve a minimum **F1-score of 0.59** to meet performance criteria.
- Compare **F1-score with AUC-ROC** to evaluate model effectiveness.
- Implement and analyze different techniques for handling class imbalance.

## Dataset
The dataset consists of customer information, banking activity, and churn status. The target variable **Exited** indicates whether a customer has left the bank (1: churned, 0: retained). Key features include:
- **CreditScore** – Creditworthiness of the customer.
- **Geography** – Country of residence.
- **Gender** – Male or female.
- **Age** – Customer's age.
- **Balance** – Account balance amount.
- **NumOfProducts** – Number of banking products used.
- **IsActiveMember** – Customer engagement level.
- **Other banking activity features** relevant to churn prediction.

## Methodology
1. **Data Preprocessing**
   - Identified and handled missing values.
   - Removed irrelevant columns (e.g., Customer ID, Surname) to prevent data leakage.
   - Encoded categorical variables using one-hot encoding.
   - Scaled numerical features to standardize the data distribution.
2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of key features.
   - Identified correlations between features and churn.
   - Discovered a **class imbalance** where ~80% of customers were retained and ~20% churned.
3. **Baseline Model**
   - Trained initial models without addressing class imbalance.
   - Observed poor recall for the minority class, highlighting the need for imbalance handling.
4. **Class Imbalance Handling**
   - Implemented **oversampling** by increasing minority class data points.
   - Applied **class weighting** to assign higher importance to churn cases during training.
5. **Model Training & Evaluation**
   - Tested multiple models, including:
     - **DecisionTreeClassifier** – Simple and interpretable baseline.
     - **RandomForestClassifier** – Improved performance via ensemble learning.
   - Conducted **hyperparameter tuning** using cross-validation.
6. **Final Testing**
   - Evaluated the best model’s performance on an unseen test dataset.
   - Compared **F1-score and AUC-ROC** to ensure both precision and recall were balanced.

## Results
- **F1-score: 0.906** – Achieved after optimization.
- **AUC-ROC: 0.944** – Provided a complementary measure of performance.
- Addressing class imbalance improved model performance significantly.

## Key Takeaways
- Feature selection and data preprocessing were crucial in improving model accuracy.
- Handling class imbalance with **oversampling and class weighting** led to better recall for churn cases.
- **Hyperparameter tuning** played a key role in model optimization.
- **RandomForestClassifier** outperformed other models in terms of generalization ability.
- Feature importance analysis revealed that **Age, Balance, and Number of Products** were strong indicators of churn.

## Technologies Used
- **Python** – Core programming language.
- **Scikit-learn** – Model training and evaluation.
- **Matplotlib & Seaborn** – Data visualization.
- **Pandas & NumPy** – Data manipulation.
