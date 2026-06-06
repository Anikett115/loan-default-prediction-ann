# Loan Default Prediction using Artificial Neural Networks (ANN)

## Project Overview

Loan defaults are one of the major challenges faced by banks and financial institutions. Accurately identifying high-risk borrowers before approving loans can significantly reduce financial losses and improve portfolio quality.

This project develops a **Loan Default Prediction System** using an **Artificial Neural Network (ANN)** built with **TensorFlow/Keras**. The model analyzes borrower information and predicts whether a loan is likely to be **Fully Paid** or **Charged Off (Default)**.

The project covers the complete machine learning workflow, including:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Categorical Encoding
* Feature Scaling
* ANN Model Development
* Model Evaluation

---

## Key Achievements

* Built an Artificial Neural Network (ANN) for loan default prediction.
* Performed extensive data cleaning and feature engineering.
* Processed over 300,000 loan records from the LendingClub dataset.
* Achieved **89% overall accuracy**.
* Achieved **93% F1-Score** for the default class.
* Achieved **100% Recall** for the default class.
* Conducted Exploratory Data Analysis to identify key loan risk factors.

---

## Business Problem

Financial institutions face significant losses when borrowers fail to repay loans.

Traditional rule-based credit scoring systems often struggle to capture complex patterns hidden within borrower data.

Machine Learning can help lenders:

* Reduce default-related losses
* Improve credit risk assessment
* Automate loan approval decisions
* Identify high-risk borrowers early
* Improve lending portfolio performance

The objective of this project is to build a predictive model capable of classifying borrowers into:

* **Fully Paid**
* **Charged Off (Default)**

---

## Project Objectives

* Clean and preprocess real-world lending data.
* Handle missing values and inconsistent records.
* Engineer meaningful predictive features.
* Analyze relationships between borrower characteristics and loan outcomes.
* Build and train an Artificial Neural Network.
* Evaluate model performance using classification metrics.
* Predict potential loan defaults.

---

## Dataset

**Dataset Source:** LendingClub Loan Dataset

The dataset contains information about borrowers and issued loans, including:

* Loan Amount
* Interest Rate
* Annual Income
* Debt-to-Income Ratio (DTI)
* Revolving Balance
* Revolving Utilization
* Public Records
* Public Record Bankruptcies
* Employment Length
* Loan Grade
* Loan Sub-Grade
* Mortgage Accounts
* Total Accounts

### Target Variable

**loan_status**

* Fully Paid
* Charged Off

---

## Technologies Used

| Category                | Technology          |
| ----------------------- | ------------------- |
| Programming Language    | Python              |
| Data Manipulation       | Pandas, NumPy       |
| Data Visualization      | Matplotlib, Seaborn |
| Machine Learning        | Scikit-Learn        |
| Deep Learning           | TensorFlow, Keras   |
| Development Environment | Jupyter Notebook    |

---

## Skills Demonstrated

* Data Cleaning
* Data Preprocessing
* Feature Engineering
* Exploratory Data Analysis (EDA)
* Data Visualization
* Feature Scaling
* Classification Modeling
* Artificial Neural Networks (ANN)
* Deep Learning
* Model Evaluation
* TensorFlow/Keras
* Scikit-Learn
* Python Programming

---

## Project Workflow

### 1. Data Cleaning

* Removed irrelevant columns.
* Handled missing values.
* Removed duplicate records.
* Corrected inconsistent categorical values.

### 2. Exploratory Data Analysis (EDA)

* Correlation Analysis
* Target Variable Analysis
* Employment Length Analysis
* Loan Grade Analysis
* Feature Relationship Visualization

### 3. Feature Engineering

* Categorical Encoding
* Dummy Variable Creation
* Feature Selection
* Removal of highly correlated variables

### 4. Data Preparation

* Train-Test Split
* Feature Scaling using StandardScaler

### 5. ANN Model Development

Model Architecture:

* Input Layer
* Hidden Dense Layers
* ReLU Activation Function
* Output Layer with Sigmoid Activation

### 6. Model Evaluation

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Classification Report

---

## Why Artificial Neural Networks?

Artificial Neural Networks are capable of capturing complex non-linear relationships that traditional statistical methods may fail to identify.

In loan default prediction, ANN models can learn hidden patterns among borrower characteristics such as:

* Income
* Debt Ratios
* Credit History
* Loan Grades
* Repayment Behavior

This makes ANN an effective solution for credit risk assessment and default prediction.

---

# Exploratory Data Analysis

## Correlation Heatmap

The correlation heatmap was used to identify relationships among numerical features.

### Key Findings

* Loan Amount and Installment show a very strong positive correlation.
* Public Records and Public Record Bankruptcies are strongly related.
* Most variables exhibit low-to-moderate correlation, reducing multicollinearity concerns.

![Correlation Heatmap](images/Correlation%20Heatmap.jpeg)

---

## Feature Correlation with Target Variable

This analysis identifies the variables most associated with loan repayment behavior.

### Key Findings

* Interest Rate has the strongest negative relationship with repayment.
* Annual Income positively influences repayment probability.
* Revolving Utilization and DTI negatively impact repayment likelihood.

![Feature Correlation](images/Correlation%20with%20Target.jpeg)

---

## Employment Length vs Loan Status

Employment stability is often considered an indicator of creditworthiness.

### Key Findings

* Borrowers with longer employment histories tend to repay loans more frequently.
* Most borrowers have more than 10 years of employment experience.
* Fully Paid loans consistently outnumber Charged Off loans across employment categories.

![Employment Length Analysis](images/Employment%20Length%20vs%20Loan%20Status.jpeg)

---

## Loan Sub-Grade Analysis

Loan grades represent borrower credit quality and risk level.

### Key Findings

* Lower-risk grades show significantly higher repayment counts.
* Higher-risk grades exhibit increased default rates.
* Loan grading provides valuable predictive information.

![Sub Grade Analysis](images/Sub-grade%20Analysis.jpeg)

---

# Model Evaluation

## Classification Report and Confusion Matrix

The ANN model was evaluated using standard classification metrics.

### Performance Summary

| Metric                    | Value |
| ------------------------- | ----- |
| Accuracy                  | 89%   |
| Precision (Default Class) | 88%   |
| Recall (Default Class)    | 100%  |
| F1 Score (Default Class)  | 93%   |

### Interpretation

* Successfully identifies the majority of default cases.
* High recall minimizes the risk of approving high-risk borrowers.
* Strong F1-score demonstrates a good balance between precision and recall.
* The model shows strong potential for real-world credit risk assessment.

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
└── LICENSE
```

---

## Installation and Usage

Clone the repository:

```bash
git clone https://github.com/Anikett115/loan-default-prediction-ann.git
```

Navigate to the project folder:

```bash
cd loan-default-prediction-ann
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

Launch Jupyter Notebook:

```bash
jupyter notebook loan_default_prediction_ann.ipynb
```

---

## Results

The developed ANN model demonstrated strong predictive capability in identifying loan repayment outcomes.

Key performance indicators include:

* 89% Overall Accuracy
* 93% F1-Score for the default class
* 100% Recall for the default class
* Strong balance between precision and recall

The high recall achieved by the model is particularly valuable in financial risk assessment because it minimizes the likelihood of approving high-risk borrowers who may eventually default on their loans.

---

## Future Improvements

* Hyperparameter Optimization
* Cross-Validation
* Ensemble Learning Models
* XGBoost Comparison
* Streamlit Web Application
* Real-Time Prediction Dashboard
* Cloud Deployment

---

## Repository Topics

Recommended GitHub Topics:

* machine-learning
* deep-learning
* tensorflow
* keras
* python
* data-science
* loan-default-prediction
* credit-risk-analysis
* classification
* feature-engineering
* exploratory-data-analysis
* artificial-neural-networks

---

## Author

**Aniket Aman**

Aspiring Data Analyst | Machine Learning Enthusiast

GitHub: https://github.com/Anikett115
