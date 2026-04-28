Loan Default Prediction System

This project is developed as part of Project Based Learning (PBL). The objective is to build a machine learning system that predicts whether giving a loan to an applicant is safe or risky.

Problem Statement  
Automated Credit Risk Categorization for Loan Approval  
Statement: Financial institutions must automate the screening of applicants while 
minimizing default risks. Students will create an applicant dataset featuring 
Credit_Score, Annual_Income, and Debt_to_Income_Ratio. The pipeline includes Data 
Balancing (SMOTE or Oversampling) to address the minority "Default" class and a 
Logistic Regression model.  
Pipeline: Applicant Profiling --> Data Balancing --> Logistic Regression --> F1
Score/Precision Evaluation.  
Project Structure  

Phase 1: Exploratory Data Analysis (EDA)  
- Data cleaning and preprocessing  
- Handling missing values  
- Converting categorical data using encoding  
- Understanding important features using basic analysis  

Phase 2: Model Training and Feature Selection  
- Logistic Regression used as baseline model  
- Feature selection techniques used:
  - Forward Selection  
  - Backward Elimination  
- PCA (Principal Component Analysis) applied for dimensionality reduction  
- Model evaluation using:
  - Recall  
  - F1 Score  
  - Confusion Matrix  
- Focus was on minimizing false negatives (important for loan default prediction)

Phase 3: User Input and Prediction  
- System takes input values from user  
- Applies same preprocessing steps  
- Predicts whether loan is:
  - Safe (0)  
  - Risky (1)  
- Separate input pipelines created for models  

Models Used  
- Logistic Regression  
- K-Nearest Neighbours (KNN)  
- Support Vector Machine (SVM)  

Key Concepts Used  
- Data preprocessing and encoding  
- Feature scaling (StandardScaler)  
- Feature selection  
- Dimensionality reduction (PCA)  
- Hyperparameter tuning  
- Model evaluation metrics  

Evaluation Metrics  

Confusion Matrix Terms  
- TP: Correctly predicted defaulters  
- TN: Correctly predicted safe applicants  
- FP: Safe predicted as risky  
- FN: Risky predicted as safe  

Metrics Used  
- Recall = TP / (TP + FN)  
- Precision = TP / (TP + FP)  
- F1 Score = 2 * (Precision * Recall) / (Precision + Recall)  

Recall was given highest importance because missing a defaulter (false negative) leads to financial loss.

Conclusion  
Different models were tested and compared. Logistic Regression was used as a baseline model. KNN was used to capture similarity between data points. SVM with RBF kernel performed best as it handled non-linear relationships effectively and gave better recall and F1 score.

The project shows how machine learning can be used to support data-driven decision making in loan approval systems.

Requirements  
- Python  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

How to Run  
1. Run Phase 1 files for data understanding  
2. Run Phase 2 files for training models  
3. Run Phase 3 files to test predictions using user input  
