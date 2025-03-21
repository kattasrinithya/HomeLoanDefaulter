🏡 Home Loan Defaulter Prediction  

Project Overview  
This project aims to predict potential home loan defaulters using machine learning techniques. By analyzing customer demographic, financial, and credit history data, the model helps financial institutions assess risk and make informed lending decisions.  

Dataset  
- The dataset contains 307,511 records with 68 features after preprocessing.  
- No missing values exist in the dataset.  
- Features include income, credit amount, employment history, previous defaults, and credit behavior.  

Exploratory Data Analysis (EDA) Insights  
- Loan defaulters tend to have lower income and higher loan-to-income ratios.  
- Customers with longer employment gaps and older age groups show higher default rates.  
- Credit bureau-related features and external risk scores (EXT_SOURCE) strongly impact loan default probability.  

Data Preprocessing  
- Feature Selection: Removed highly correlated and redundant features.  
- Encoding Techniques: Label Encoding, Frequency Encoding, and Ordinal Encoding were used for categorical variables.  
- Scaling: MinMaxScaler applied to numerical features for better model performance.  

Machine Learning Models Evaluated  
Model                  | Accuracy  | AUC-ROC Score  
------------------------|-----------|---------------  
Gradient Boosting      | 91.90% | 0.76  
Random Forest         | 91.85%    | 0.69  
Decision Tree         | 91.37%    | 0.70  
XGBoost              | 86.43%    | 0.74  
Logistic Regression   | 69.41%    | 0.73  

Best Performing Model  
The Gradient Boosting Model achieved the highest accuracy and AUC-ROC score, making it the most reliable model for predicting loan defaults.  

Key Challenges & Solutions  
- Class Imbalance: Used class_weight='balanced' and computed sample weights to improve minority class representation.  
- Overfitting in Decision Trees: Applied hyperparameter tuning and pruning techniques.  
- Feature Importance Analysis: Dropped less significant and highly correlated features to reduce noise.  

Business Impact  
This predictive model can help financial institutions:  
- Reduce loan default risks by identifying high-risk applicants.  
- Optimize loan approval processes with data-driven decisions.  
- Improve customer targeting strategies for better risk assessment.  

Future Improvements  
- Implement deep learning models (Neural Networks) for better performance.  
- Explore cost-sensitive learning techniques to enhance minority class predictions.  
- Fine-tune hyperparameters further using Bayesian Optimization.  
