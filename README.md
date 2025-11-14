## CIND119 – Customer Churn Prediction (REES46 E-Commerce Dataset)

This repository contains all code, analysis, visualizations, and documentation for my CIND119 Applied Research Project at Toronto Metropolitan University.
The project focuses on predicting customer churn using the REES46 e-commerce behavioral dataset and comparing two machine-learning models: Decision Tree and Naïve Bayes.


# Project Overview

The purpose of this project is to analyze behavioral patterns in e-commerce activity and develop machine-learning models that predict whether a user will churn.

The REES46 dataset includes:

- Session behavior
- Purchase activity
- Clickstream-derived features
- Recency, frequency, monetary (RFM) metrics
- Latent preference embeddings
- Churn indicator (target_event)

  # Project Stages:

  ## Milestone 1 – Research Question & Abstract:
- Defined the problem: predicting customer churn in a non-contractual e-commerce environment
- Conducted preliminary literature review
- Wrote the initial abstract and project scope


  ## Milestone 2 - Milestone 2 – Literature Review, Data Description & Project Approach
  ### Literature review
- Reviewed recent academic work on churn prediction
- Observed the importance of behavioral features (RFM)
- Justified the choice of Decision Tree & Naïve Bayes for interpretability and baseline comparison

  ### Data Description
- Loaded and examined the REES46 aggregated behavioral dataset
- Produced summary statistics, missing value checks, skewness analysis
- Identified Recency, Frequency, Monetary, and Latent features
- Generated correlation heatmaps and distribution plots

  ### Project Approach
  - Prepared modeling pipeline
  - Removed leakage variables (target_actual_profit, target_revenue, etc.)
  - Planned feature selection (Mutual Information
  - Planned handling of class imbalance (SMOTE)
 
  ## Milestone 3 – Modeling, Evaluation & Insights
  ### Model Development
  Built two pipelines using:
    - SMOTE for balancing
    - SelectKBest (Mutual Information) for feature selection
    - Decision Tree Classifier
    - Gaussian Naïve Bayes
  ### Evaluation Methods
  - Holdout split (80/20) for real-world simulation
  - 5-fold Stratified Cross-Validation for stability
