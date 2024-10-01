# SecureSwipe: Credit Card Fraud Detection (Year 3 Sem 1) (2023)

## Project Overview

SecureSwipe is a machine learning solution developed to enhance the detection of credit card fraud. With the growing threat of cybercrimes, particularly credit card fraud, we aim to protect financial institutions, merchants, and customers by improving the accuracy and reliability of fraud detection systems. This project leverages various machine learning algorithms to minimize false positives and maximize the detection of fraudulent transactions.

## Files in this Repository

- **`bs_dataset.csv`**: The dataset used for this project, sourced from Kaggle's BankSim dataset.
- **`feature_selection_2nd_try (1).ipynb`**: A Jupyter notebook where the team conducted feature selection using various techniques.
- **`EDA.ipynb`**: A Jupyter notebook focused on exploratory data analysis (EDA) to understand the dataset's structure, identify trends, and clean the data.
- **`Model.ipynb`**: The notebook containing the code for building and evaluating machine learning models.

## Project Structure

### 1. Exploratory Data Analysis (EDA)
- Analyzed the dataset to detect any missing values, understand summary statistics, and visualize trends.
- Focused on identifying age groups and categories (such as leisure and travel) associated with higher levels of fraudulent transactions.
- Found a significant imbalance between fraudulent and non-fraudulent transactions, requiring oversampling with SMOTE to balance the dataset.

### 2. Data Preprocessing
- Performed data cleaning by removing ambiguous values.
- Applied encoding techniques such as Label Encoding and One-Hot Encoding for categorical features.
- Feature selection techniques like Variance Threshold, K-best features, Recursive Feature Elimination, and Boruta were used, but most features were retained for modeling.

### 3. Handling Class Imbalance
- Addressed the significant imbalance between fraud and non-fraud transactions (1:82 ratio) using SMOTE, a synthetic oversampling method, to balance the dataset.

### 4. Model Building
We experimented with several machine learning models to detect fraudulent transactions, including:
- **Random Forest Classifier**: Chosen for its high accuracy and ability to handle large datasets.
- **Artificial Neural Network (ANN)**: Used for its flexibility and adaptability to complex patterns in the dataset.
- **Ensemble Model (Stacking)**: Combined predictions from Random Forest and ANN with a meta-model (Logistic Regression) for improved performance.

### 5. Model Evaluation
- The models were evaluated using common classification metrics such as accuracy, precision, recall, and F1-score.
- We focused on the F1-score as it provides a more balanced evaluation between fraud and non-fraud classification performance.
- **Random Forest** achieved a high recall for fraud detection, making it one of the better-performing models.

## Results
- The Random Forest model performed well with a high recall for fraudulent transactions.
- The stacked ensemble model combining Random Forest and ANN, with Logistic Regression as the meta-model, demonstrated improved overall performance in fraud detection.

---

This project showcases the potential of machine learning to enhance fraud detection systems. The final model balances the trade-offs between precision and recall, ensuring robust protection for financial institutions and customers alike.
