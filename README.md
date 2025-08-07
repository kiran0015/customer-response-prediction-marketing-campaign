# Customer Response Prediction for Marketing Campaign

This project presents a comprehensive analysis of the **Bank Marketing Dataset** from the UCI Machine Learning Repository. It combines both **exploratory data analysis (EDA)** and **machine learning classification** to predict whether a client will subscribe to a term deposit based on various demographic and campaign-related features. 
We also designed a professional **Excel Dashboard** to make marketing insights accessible to business teams.

## Problem Statement

A Portuguese banking institution conducted direct marketing campaigns through phone calls to sell term deposits. The dataset includes information on client profiles, past marketing interactions, and external economic indicators. 

The objective is to predict if a client will subscribe to a term deposit (`y` = 'yes' or 'no'), and to derive key customer insights for improved campaign strategies.

## Dataset Information
•	Source: UCI Machine Learning Repository – Bank Marketing Dataset

•	File: uci_bank_marketing_cleaned.xlsx

•	Size: Cleaned version with irrelevant columns removed and NA-handling applied

•	Rows: ~41,000

•	Target Variable: y (binary: 'yes' or 'no')

•	Key Features Used

          Demographics: Age, Job, Marital status, Education
          
          Financial Indicators: Default, Housing, Loan
          
          Campaign Details: Contact method, Month, Campaign interactions
          
          Economic Indicators: Employment variation rate, consumer price index, etc
          
## Project Workflow
1.	Data Cleaning: Removed columns like duration, deposit; Label Encoding & OneHot Encoding for categorical variables
2.	EDA: Visualized key variables such as age, job, marital status, and campaign outcomes;	Investigated relationships between customer traits and subscription likelihood
3.	Feature Engineering:	Used ColumnTransformer for preprocessing;	Applied one-hot encoding and scaling
4.	Class Balancing:	SMOTE (Synthetic Minority Oversampling Technique);	class_weight="balanced" in model training
5.	Built and evaluated multiple models: Logistic Regression; Decision Tree;	XGBoost
6.	Hyperparameter tuning using GridSearchCV
7.	Evaluation Metrics:	Accuracy,	Precision,	Recall,	F1 Score,	ROC AUC Curve
   
## Files Included

 uci_bank_marketing_cleaned.xlsx: Cleaned dataset used in Excel dashboard
 
 uci_bank_marketing.ipynb: Python notebook with preprocessing, model training, and evaluation
 
 Excel Dashboard Images (.png): Screenshots of the final Excel dashboard with slicers and charts
 

## 📈 Excel Dashboard Highlights

The Excel Dashboard offers a powerful business view of customer segments and campaign results.

### Key Features:
- Slicers for Job, Marital Status, Education, and Month
- KPI Cards: Total Customers, Subscription Rate, Campaign Success Rate
- Visuals: 
  - Term Subscription by Job
  - Campaign Outcome by Age Group
  - Pie Chart for Marital Status vs Outcome
  - Month-wise Trend Analysis


### Key Insights

- Marital Status and Job Type significantly impact term deposit subscription.
- Campaigns in May and August saw the highest call volumes.
- Customers aged 30–40 had the highest conversion rate.
- Students and retired individuals are more likely to subscribe.
 

## Results Summary
- Model            	   Accuracy	Precision	Recall	F1 Score
- Logistic Regression	  79 %	    62%     73%       64%
- Decision Tree	        87%     	69%	    74%     	71%
- XGBoost             	90%	      77%	    63%	      67%
				
### Tools & Technologies
-	Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Google Colab
- Excel 
________________________________________
 ## Learnings
-	Importance of preprocessing and class balancing in imbalanced datasets
-	Comparative performance of traditional ML vs ensemble models
-	Interpreting model metrics in a business context

