# Loan Default Prediction using Artificial Neural Networks (ANN)

## Project Overview

Financial institutions face significant losses due to loan defaults. Identifying high-risk borrowers before loan approval is a critical business problem in the banking and lending industry.

This project develops a Loan Default Prediction System using an Artificial Neural Network (ANN) built with TensorFlow/Keras. The model analyzes borrower information and predicts whether a loan is likely to be repaid or defaulted.

The project includes extensive data cleaning, exploratory data analysis (EDA), feature engineering, categorical encoding, feature scaling, and ANN model development.

---
## Key Achievements

- Built an Artificial Neural Network (ANN) for loan default prediction
- Performed extensive data cleaning and feature engineering
- Processed 300,000+ loan records from the LendingClub dataset
- Achieved 89% classification accuracy
- Achieved 93% F1-Score for the default class
- Conducted Exploratory Data Analysis (EDA) to identify risk factors
---

## Business Problem

Loan defaults create substantial financial risk for lenders.

Traditional rule-based systems may fail to capture complex patterns in borrower behavior. Machine Learning models can help lenders:

- Reduce financial losses
- Improve credit risk assessment
- Automate loan approval decisions
- Identify high-risk applicants early
- Improve portfolio quality

The objective of this project is to build a predictive model capable of classifying loan applicants into:

- Fully Paid
- Charged Off (Default)

---

## Project Objectives

- Perform extensive data cleaning and preprocessing
- Handle missing values and inconsistent records
- Engineer meaningful predictive features
- Analyze relationships between borrower characteristics and loan outcomes
- Train an Artificial Neural Network using TensorFlow/Keras
- Evaluate model performance using classification metrics
- Predict potential loan defaults

---

## Dataset

**Source:** LendingClub Loan Dataset

The dataset contains borrower information such as:

- Loan Amount
- Interest Rate
- Annual Income
- Debt-to-Income Ratio
- Revolving Balance
- Public Records
- Employment Length
- Loan Grade
- Loan Sub-grade
- Mortgage Accounts
- Total Accounts

Target Variable:

- Loan Status (Fully Paid / Charged Off)

---

## Technologies Used

| Category | Technologies |
|-----------|------------|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn |
| Deep Learning | TensorFlow, Keras |
| Notebook Environment | Jupyter Notebook |

---

## Project Workflow

### 1. Data Cleaning

- Removed irrelevant features
- Handled missing values
- Removed duplicate records
- Fixed inconsistent categorical values

### 2. Exploratory Data Analysis (EDA)

- Correlation Analysis
- Target Distribution Analysis
- Employment Length Analysis
- Loan Grade Analysis
- Feature Relationship Visualization

### 3. Feature Engineering

- Categorical Encoding
- Dummy Variable Creation
- Feature Selection
- Removal of highly correlated variables

### 4. Data Preparation

- Train-Test Split
- Feature Scaling using StandardScaler

### 5. ANN Model Development

Artificial Neural Network Architecture:

- Input Layer
- Hidden Dense Layers
- ReLU Activation
- Output Layer with Sigmoid Activation

### 6. Model Evaluation

Metrics Used:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

# Exploratory Data Analysis

## Correlation Heatmap

The correlation heatmap was used to identify relationships among numerical features.

### Key Findings

- Loan Amount and Installment show very strong positive correlation.
- Public Records and Public Record Bankruptcies are highly related.
- Most features show low-to-moderate correlation, reducing multicollinearity concerns.

![Correlation Heatmap](images/Correlation%20Heatmap.jpeg)

---

## Feature Correlation with Target Variable

This analysis identifies the variables most associated with loan repayment behavior.

### Key Findings

- Interest Rate has the strongest negative relationship with repayment.
- Annual Income positively influences repayment probability.
- Revolving Utilization and DTI negatively impact repayment likelihood.

![Feature Correlation](images/Correlation%20with%20Target.jpeg)

---

## Employment Length vs Loan Status

Employment stability is often considered an indicator of creditworthiness.

### Key Findings

- Borrowers with longer employment histories tend to repay loans more frequently.
- The majority of borrowers have 10+ years of employment experience.
- Fully Paid loans consistently outnumber Charged Off loans across all employment categories.

![Employment Length Analysis](images/Employment%20Length%20vs%20Loan%20Status.jpeg)

---

## Loan Sub-Grade Analysis

Loan grades are assigned based on borrower credit risk.

### Key Findings

- Lower-risk grades show significantly higher repayment counts.
- Higher-risk grades exhibit increased default rates.
- Loan grading provides valuable predictive information.

![Sub Grade Analysis](images/Sub-grade%20Analysis.jpeg)

---

# Model Evaluation

## Classification Report and Confusion Matrix

The ANN model was evaluated using standard classification metrics.

### Performance Summary

| Metric | Value |
|----------|---------|
| Accuracy | 89% |
| Precision (Default Class) | 88% |
| Recall (Default Class) | 100% |
| F1 Score (Default Class) | 93% |

### Interpretation

- The model successfully identifies the majority of default cases.
- High recall minimizes the risk of approving high-risk borrowers.
- Strong F1-score indicates a good balance between precision and recall.

![Model Evaluation](images/ClassificationReport%20and%20ConfusionMatrix.png)

---

## Project Structure

```text
loan-default-prediction-ann/
│
├── images/
│   ├── ClassificationReport and ConfusionMatrix.png
│   ├── Correlation Heatmap.jpeg
│   ├── Correlation with Target.jpeg
│   ├── Employment Length vs Loan Status.jpeg
│   └── Sub-grade Analysis.jpeg
│
├── loan_default_prediction_ann.ipynb
├── README.md
├── LICENSE
```

---
## Skills Demonstrated

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Data Visualization
- Feature Scaling
- Artificial Neural Networks
- Classification Modeling
- Model Evaluation
- TensorFlow/Keras
- Scikit-Learn
---

## Results

The Artificial Neural Network successfully classified loan applicants into default and non-default categories.

The project demonstrates how Deep Learning can assist financial institutions in:

- Credit Risk Assessment
- Loan Approval Decision Making
- Portfolio Risk Management
- Default Prevention

The model achieved strong predictive performance while maintaining high recall for default identification.

---

## Future Improvements

- Hyperparameter Optimization
- Cross-Validation
- Ensemble Models
- XGBoost Comparison
- Deployment using Flask/FastAPI
- Real-Time Prediction Dashboard

---

## Author

**Aniket Aman**

Aspiring Data Analyst / Machine Learning Enthusiast

GitHub: https://github.com/Anikett115
