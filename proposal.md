# CSC172 Association Rule Mining Project Proposal
**Student:** [Your Name], [ID]  
**Date:** [Submission Date]

## 1. Project Title 
Market Basket Analysis using Apriori Algorithm


## 2. Problem Statement
Retail businesses need to identify product co-purchase patterns to optimize shelf placement, bundling, and cross-selling strategies. This project analyzes transactional data to discover frequent itemsets and strong association rules. Locally relevant for Philippine retail chains and sari-sari stores analyzing customer buying behavior.

## 3. Objectives
- Preprocess transactional data and perform EDA with visualizations
- Implement Apriori algorithm to generate association rules
- Evaluate rules using support, confidence, lift, and conviction metrics

## 4. Dataset Plan
- Source: [Groceries Dataset - Kaggle](https://www.kaggle.com/datasets/heeraldedhia/groceries-dataset) (~10K transactions, 169 items)
- Domain: Grocery retail transactions
- Acquisition: Direct Kaggle download to `data/groceries.csv`

## 5. Technical Approach
- Preprocessing: One-hot encoding → mlxtend TransactionEncoder
- Algorithm: Apriori (min_support=0.02, min_confidence=0.6, min_lift=1.2)
- Framework: Python + pandas + mlxtend + matplotlib/seaborn
- Environment: Jupyter Notebook / Google Colab

## 6. Expected Challenges & Mitigations
- Challenge: Sparse transaction matrix
- Solution: Filter infrequent items (support > 0.01)
  
- Challenge: Long Apriori runtime
- Solution: Limit max itemset length to 3
  
- Challenge: Trivial rules
- Solution: High lift threshold (>1.2)
