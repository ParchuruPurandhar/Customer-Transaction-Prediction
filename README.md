# Customer Transaction Prediction using Machine Learning
## Project Overview

Customer transaction prediction is an important machine learning application in banking, finance, and retail industries. This project aims to predict whether a customer will perform a transaction based on historical customer data and anonymized numerical features.

The project compares multiple supervised machine learning algorithms and identifies the best-performing model through evaluation and hyperparameter tuning.

#### Objective

The primary objectives of this project are:

  » Predict whether a customer will make a transaction.
  » Compare the performance of multiple machine learning algorithms.
  » Improve model performance using hyperparameter tuning.
  » Identify the most suitable model for deployment.
#### Dataset Information

The dataset contains:

  » 200 anonymized numerical features (var_0 to var_199)
  » ID column: ID_code
  » Target column: target

#### Target Values:

Value	Meaning
  » 0	No Transaction
  » 1	Transaction Occurred
  
### Project Workflow

Data Collection
       ↓
Data Understanding
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis (EDA)
       ↓
Feature Selection
       ↓
Train-Test Split
       ↓
Feature Scaling
       ↓
Model Training
       ↓
Hyperparameter Tuning
       ↓
Model Evaluation
       ↓
Best Model Selection


### Technologies Used
#### Programming Language
    Python
#### Libraries
    NumPy
    Pandas
    Matplotlib
    Seaborn
    Scikit-Learn
    XGBoost
### Exploratory Data Analysis
The following analyses were performed:

    Data Quality Checks
    Checked dataset shape and structure
    Verified data types
    Checked missing values
    Statistical summary generation
    Visualizations
    Feature distributions
    Histograms
    Boxplots
    Target variable distribution
    Correlation heatmap
#### Key Findings

    Dataset contains no missing values.
    Features are already standardized/anonymized.
    Target variable is imbalanced.
    Most features show low correlation with each other.
    Several features contain useful outliers that should be retained.
### Data Preprocessing

    Removed ID_code column.
    Split data into training and testing sets.
    Applied Standard Scaling using StandardScaler.
    from sklearn.preprocessing import StandardScaler
    scaler = StandardScaler()
    X_train = scaler.fit_transform(X_train)
    X_test = scaler.transform(X_test)

#### Machine Learning Models Implemented

1. Logistic Regression
      Simple baseline model
      Fast training and prediction
2. Decision Tree
      Easy interpretability
      Captures nonlinear relationships
3. Support Vector Machine (Linear SVC)
      Effective in high-dimensional spaces
      Good classification performance
4. Random Forest
      Ensemble learning approach
      Reduces overfitting
      Handles feature interactions effectively
5. XGBoost
      gradient boosting algorithm
      High predictive performance
      Handles complex patterns efficiently
   
### Model Evaluation Metrics

##### The following metrics were used:

    Accuracy
    Precision
    Recall
    F1 Score

##### Since the dataset is imbalanced, greater importance was given to:
    Precision
    Recall
    F1 Score
  
### Hyperparameter Tuning

GridSearchCV was used to optimize:

#### Ⅰ Logistic Regression

    Penalty
    C value
    Max iterations
#### Ⅱ Decision Tree
    Criterion
    Max depth
    Min samples split
    Min samples leaf
#### Ⅲ SVM
    C value
    Loss function
#### Ⅳ Random Forest
    Number of estimators
    Max depth
    Min samples split
    Min samples leaf
#### Ⅴ XGBoost
    Number of estimators
    Learning rate
    Max depth
### Results - Model Comparison
  The performance of all models was compared before and after tuning.
  Best Performing Model

🏆 XGBoost

### Reasons:

    1. Highest overall predictive performance
    2. Strong F1 Score
    3. Better handling of complex feature interactions
    4. Suitable for large-scale deployment
### Business Insights

    1. Machine learning can effectively predict customer transaction behavior.
    2. High-risk customers can be identified in advance.
    3. Businesses can improve marketing campaigns using prediction results.
    4. Resource allocation and customer targeting can be optimized.
### Challenges Faced

    1. Handling feature scaling requirements across different algorithms.
    2. Selecting the most appropriate model among multiple candidates.
    3. Increased computation time during hyperparameter tuning.
    4. Managing the trade-off between accuracy and model complexity.
### Limitations

    1. Target class imbalance may affect minority class prediction.
    2. Features are anonymized, limiting business interpretation.
    3. Performance depends on the quality of historical transaction data.
### Future Improvements

    1. Apply SMOTE for class imbalance handling.
    2. Perform feature engineering.
    3. Explore PCA for dimensionality reduction.
    4. Experiment with Deep Learning models.

### Author

# Parchuru Purandhar

## Machine Learning Project – Customer Transaction Prediction
