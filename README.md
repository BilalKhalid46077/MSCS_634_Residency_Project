# MSCS_634_ProjectDeliverable_1

## Project Overview

This repository contains Deliverable 1 of the Advanced Data Mining Project. The objective is to prepare a real-world dataset for future machine learning tasks by performing data loading, cleaning, preprocessing, and exploratory data analysis.

## Dataset

Online Shoppers Purchasing Intention Dataset

Source:
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

Records: 12,330

Features: 18

## Data Cleaning

- Loaded dataset using Pandas
- Examined dataset structure
- Checked missing values
- Removed duplicate records
- Examined numerical and categorical features
- Identified potential outliers

## Exploratory Data Analysis

Several visualizations were created including:

- Histograms
- Count plots
- Correlation heatmap
- Boxplots
- Pairplots

These visualizations helped understand customer purchasing behavior and relationships among variables.

## Key Insights

- Most visitors did not complete a purchase.
- Returning visitors represented a large portion of website traffic.
- Some browsing features showed moderate relationships with purchasing behavior.
- A small number of outliers were identified in browsing duration.

## Challenges

The primary challenge was understanding the dataset structure and selecting appropriate visualizations. Duplicate records were removed to improve data quality before future modeling tasks.

## Next Steps

The cleaned dataset will be used in Deliverable 2 for feature engineering, regression modeling, and performance evaluation.

# MSCS_634_ProjectDeliverable_2
**Project Deliverable:** 2 – Regression Modeling and Performance Evaluation

---

# Project Overview

The purpose of this project is to build and evaluate regression models using the **Online Shoppers Purchasing Intention Dataset**. The project focuses on predicting the *Administrative_Duration* variable based on other website session features.

Different regression techniques were implemented and compared to understand how feature engineering and model selection affect prediction performance. Cross-validation was also used to evaluate how well the models generalize to unseen data.

---

# Dataset

**Dataset:** Online Shoppers Purchasing Intention Dataset

The dataset contains information about visitor behavior during online shopping sessions, including:

- Administrative pages visited
- Informational pages visited
- Product-related pages visited
- Time spent on each page type
- Bounce rates
- Exit rates
- Page values
- Visitor type
- Weekend visits
- Revenue indicator

The dataset contains more than 12,000 records and multiple numerical and categorical attributes, making it suitable for regression and predictive modeling.

---

# Feature Engineering

Several preprocessing and feature engineering steps were performed before model training:

- Removed missing values (if any)
- Converted categorical variables into numerical values using one-hot encoding
- Selected **Administrative_Duration** as the target variable
- Used the remaining attributes as predictor variables
- Split the dataset into training and testing sets
- Standardized numerical features using StandardScaler

These steps prepared the dataset for regression analysis and improved model performance.

---

# Model Evaluation

The models were evaluated using:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

Five-fold Cross Validation was also performed to measure how well each model generalizes to unseen data.

---

# Visualizations

The notebook includes several visualizations, including:

- Actual vs Predicted values
- Regression comparison plots
- Model performance comparison
- Cross-validation score comparison

These figures help compare the prediction performance of each regression model.

---

# Key Findings

- Linear Regression provided a strong baseline for prediction.
- Cross-validation showed that the selected models generalized well to unseen data.
- Regularization helped reduce the possibility of overfitting while maintaining stable prediction performance.

---

# Challenges Encountered

Some challenges encountered during this project included:

- Selecting an appropriate target variable for regression.
- Handling categorical variables before model training.
- Scaling numerical features for fair model comparison.
- Comparing multiple evaluation metrics to determine the best-performing model.

These challenges were addressed through proper preprocessing, feature engineering, and model evaluation techniques.

---

# Conclusion

This project demonstrated the complete regression modeling process, including feature engineering, model development, evaluation, and comparison. The results show that regression techniques can effectively model relationships within the Online Shoppers Purchasing Intention dataset, while regularization methods help improve model stability and reduce overfitting.

---

# MSCS_634_ProjectDeliverable_3

**Project Deliverable:** 3 – Classification, Clustering, and Pattern Mining

## Objective

The purpose of this deliverable is to apply different data mining techniques to classify customer purchase intentions, identify customer groups through clustering, and discover product purchasing patterns using association rule mining.

## Tasks Completed

- Developed two classification models:
  - Decision Tree
  - K-Nearest Neighbors (KNN)

- Performed hyperparameter tuning using GridSearchCV for the Decision Tree model.

- Evaluated classification models using:
  - Accuracy
  - F1 Score
  - Confusion Matrix
  - ROC Curve

- Applied K-Means clustering to identify customer groups.

- Visualized clustering results using PCA.

- Applied the Apriori algorithm to discover frequent itemsets.

- Generated association rules using:
  - Support
  - Confidence
  - Lift

## Key Findings

- The tuned Decision Tree produced better classification performance than the default model.
- KNN also achieved strong prediction accuracy but required additional computation.
- K-Means successfully grouped customers with similar browsing behavior.
- Association rule mining identified combinations of customer behaviors that frequently occurred together.
- The discovered patterns can help improve marketing strategies and customer recommendations.

## Real-World Applications

- Customer purchase prediction
- Personalized marketing
- Customer segmentation
- Recommendation systems
- Business intelligence
- Decision support

## Challenges Faced

- Selecting suitable hyperparameters for the Decision Tree.
- Preparing transactional data for association rule mining.
- Choosing an appropriate number of clusters for K-Means.

## Tools Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- mlxtend

