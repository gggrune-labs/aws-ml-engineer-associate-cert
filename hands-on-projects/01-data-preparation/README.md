# Project 1: Data Preparation Pipeline

**Week:** 1  
**Date:** March 10-14, 2026  
**Domain:** Data Preparation for ML (28%)

## Objective

Build an end-to-end data preparation pipeline that:
1. Uploads raw data to S3
2. Queries data using Athena
3. Performs feature engineering
4. Creates train/validation/test splits
5. Saves processed data to S3 in proper format for SageMaker

## Dataset

**Name:** [TBD - Titanic/Churn/Fraud]  
**Source:** Kaggle  
**Size:** ___ rows, ___ columns  
**Type:** Classification / Regression  
**Target Variable:** ___

## Architecture
```
Raw Data (CSV)
    ↓
Amazon S3 (raw-data/)
    ↓
Amazon Athena (exploratory queries)
    ↓
SageMaker Notebook (feature engineering)
    ↓
Amazon S3 (processed-data/train|val|test/)
```

## S3 Bucket Structure
```
s3://sagemaker-us-east-1-{account-id}/
└── ml-engineer-practice/
    ├── raw-data/
    │   └── data.csv
    └── processed-data/
        ├── train/
        │   └── train.csv
        ├── validation/
        │   └── validation.csv
        └── test/
            └── test.csv
```

## Feature Engineering Steps

1. **Handle Missing Values:**
   - [Strategy used]

2. **Feature Creation:**
   - [New features created]

3. **Categorical Encoding:**
   - [Encoding method]

4. **Normalization/Scaling:**
   - [If applicable]

5. **Data Split:**
   - Train: 60%
   - Validation: 20%
   - Test: 20%
   - Stratified: Yes/No

## Code

**Notebook:** [`data_prep.ipynb`](./data_prep.ipynb)  
**Processing Script:** [`preprocessing.py`](./preprocessing.py)

## Results

**Training Set Size:** ___ rows  
**Validation Set Size:** ___ rows  
**Test Set Size:** ___ rows  
**Features:** ___ columns  
**S3 Upload Success:** ✅ / ❌

## Key Learnings

1. [Learning 1]
2. [Learning 2]
3. [Learning 3]

## Next Steps

This processed data will be used in:
- **Project 2:** XGBoost Model Training
- **Project 3:** Hyperparameter Tuning

## AWS Services Used

- Amazon S3
- Amazon Athena
- Amazon SageMaker (Notebooks)
- IAM (roles and permissions)

## Cost

**Estimated:** < $1 (all within free tier)

---

**Status:** In Progress 🔄  
**Completion Date:** TBD