# FinTrust Digital Bank — Predictive Intelligence




<img width="1007" height="787" alt="Screenshot 2026-09-29 161431" src="https://github.com/user-attachments/assets/8fb36242-1e77-4bd0-96bd-54279b946923" />


## 📌 Project Overview

This repository contains my **Week 1 Data Science project** for the **AnalystLab Africa Experience Lab Internship Programme**, based on the FinTrust Digital Bank case study.

FinTrust is a fictional digital banking organisation exploring the use of **data, machine learning, and generative AI** to better understand customer and transaction behaviour, support risk-related decision-making, improve operational processes, and strengthen digital customer support.

As part of the **Data Science Track**, my Week 1 focus was on defining a predictive intelligence problem that could help FinTrust identify transactions that may require further risk review. The official assignment asks the Data Science track to define the predictive problem, assess the `Risk_Review_Flag` target, identify candidate features, formulate hypotheses, and create an initial modelling plan.

## 🎯 Problem Statement

FinTrust has a large volume of customer and transaction activity that may be difficult to review manually.

The predictive objective is to investigate whether machine learning can be used to estimate which transactions should be **flagged for risk review**, allowing potential high-risk patterns to be prioritised for further investigation.

> **Important:** `Risk_Review_Flag` is a synthetic educational label. It should not be interpreted as a real-world fraud determination.

## 🔍 Week 1 Objectives

The main objectives of this project were to:

- Understand the FinTrust business problem and the role of predictive analytics.
- Profile the available customer and transaction data.
- Investigate the `Risk_Review_Flag` field as a potential modelling target.
- Identify potential predictive features and data-quality concerns.
- Develop testable hypotheses about factors associated with the risk-review label.
- Establish an initial machine-learning workflow for future weeks.

These objectives align with the official Week 1 Data Science requirements. fileciteturn0file0L134-L160

## 📊 Data

The official FinTrust project provides the following data resources:

- `FinTrust_Customer_Data.csv`
- `FinTrust_Transaction_Data.csv`
- `FinTrust_Data_Dictionary.xlsx`

The project also provides a financial knowledge base and other project documentation. The FinTrust data is **synthetic and created for educational purposes**. fileciteturn0file0L36-L49

### Data Profiling

The Week 1 analysis focuses on understanding the datasets before extensive cleaning or modelling.

Areas investigated include:

- Number of records
- Number of columns
- Field names
- Data types
- Categorical variables
- Numerical variables
- Date/time variables
- Relationships between datasets
- Missing values
- Obvious data-quality issues

The assignment specifically states that extensive data cleaning is not required at this stage. fileciteturn0file0L83-L97

## 🎯 Target Variable

### `Risk_Review_Flag`

The target variable is assessed to determine:

- What the field represents
- Its possible values
- Whether it can be used as a modelling target
- Whether the classes are balanced or imbalanced
- Potential limitations of using the label

Because the target may be imbalanced, model evaluation should not rely only on accuracy. Metrics such as **precision, recall, F1-score, and ROC-AUC/PR-AUC** can be considered during later modelling, depending on the final target distribution.

## 💡 Initial Hypotheses

The Week 1 project develops hypotheses rather than treating them as conclusions.

Examples of areas investigated include:

1. **Transaction value** may be associated with whether a transaction receives a risk-review flag.
2. **Transaction channel** may show different risk-review patterns.
3. **Transaction status or behaviour patterns** may be associated with the risk-review label.
4. **Customer-level characteristics and transaction activity** may provide useful predictive information.

These hypotheses will need to be tested through exploratory analysis and modelling rather than assumed to be true. The official assignment requires at least three hypotheses and explicitly states that hypotheses should not be presented as conclusions. fileciteturn0file0L154-L160

## 🧠 Candidate Features

Potential predictive features are being assessed based on their relationship to transaction and customer behaviour.

Candidate feature categories include:

| Feature Category | Why It May Matter |
|---|---|
| Transaction amount | May capture unusual or high-value activity |
| Transaction channel | Different channels may have different behavioural patterns |
| Transaction status | May provide information about transaction outcomes |
| Customer attributes | May capture differences in customer behaviour |
| Transaction frequency | May identify unusual activity levels |
| Time/date features | May reveal temporal patterns |
| Account/customer activity | May provide behavioural context |
| Other transaction attributes | May capture additional risk-related signals |

The final feature set will depend on data availability, data quality, leakage checks, and exploratory findings.

## 🛠️ Tools & Technologies

The project uses or plans to use:

- **Python** — primary programming language
- **Pandas** — data manipulation and profiling
- **NumPy** — numerical analysis
- **Scikit-learn** — machine-learning workflows and evaluation
- **Jupyter Notebook analysis and experimentation
- **Git & GitHub** — version control and project documentation

These tools are consistent with the recommended Data Science tools in the Week 1 assignment. fileciteturn0file0L161-L178

## 🔄 Initial Machine Learning Workflow

The planned workflow is:

```text
Raw Data
   ↓
Data Understanding & Profiling
   ↓
Data Quality Checks
   ↓
Exploratory Data Analysis
   ↓
Data Preparation
   ↓
Feature Engineering
   ↓
Train / Validation / Test Split
   ↓
Baseline Model
   ↓
Candidate Models
   ↓
Model Evaluation
   ↓
Error Analysis
   ↓
Interpretation & Limitations
```

The modelling process will prioritise reproducibility and interpretability, while paying particular attention to class imbalance and potential data leakage.

## 📈 Evaluation Strategy

Potential evaluation metrics include:

- **Precision** — proportion of predicted review cases that are actually labelled for review.
- **Recall** — proportion of labelled review cases identified by the model.
- **F1-score** — balance between precision and recall.
- **Confusion matrix** — overview of classification errors.
- **ROC-AUC** — overall ranking ability across classification thresholds.
- **PR-AUC** — useful when the positive class is relatively rare.

The final metrics will be selected after examining the target distribution and business context.

## 🗓️ Week 1 

### Week 1 — Understand & Plan
- Business understanding
- Data profiling
- Target assessment
- Candidate feature identification
- Hypothesis development
- Initial modelling plan
