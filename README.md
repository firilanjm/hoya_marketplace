# Hoya Marketplace Analysis: Economic Potential and Explainable Machine Learning

This repository contains data collection, cleaning, exploratory analysis, and machine learning workflows for analyzing the economic potential of Hoya ornamental plants in the Indonesian online marketplace.

The project investigates marketplace activity using Shopee product listings and explores factors associated with high-revenue products through explainable machine learning techniques.

## Research Objectives

* Identify the most traded Hoya varieties.
* Analyze price variation across Hoya varieties.
* Examine geographic patterns of Hoya sales activity.
* Estimate marketplace revenue based on listing information.
* Develop predictive models for identifying high-revenue listings.
* Interpret machine learning predictions using SHAP explainability.

## Dataset

The dataset consists of Hoya product listings collected from Shopee and includes:

* Product name
* Hoya variety
* Product price
* Number sold
* Seller location
* Product rating
* Number of reviews
* Shop name
* Product URL
* Scraping date

Estimated revenue is calculated as:

Estimated Revenue = Price × Number Sold

## Repository Structure

```text
hoya_marketplace/

├── data/
│   ├── shopee_hoya_master.csv
│   └── shopee_hoya_clean.csv
│
├── notebooks/
│   ├── 00_data_cleaning.ipynb
│   ├── 01_marketplace_analytics.ipynb
│   └── 02_ml_comparison.ipynb
│
├── results/
│   ├── figure/
│   └── table/
│
├── paper/
│
├── README.md
└── .gitignore
```

## Analysis Workflow

### 1. Data Cleaning

* Filtering Hoya-related products
* Removing irrelevant listings
* Standardizing variety names
* Removing duplicate records
* Preparing analysis-ready data

### 2. Marketplace Analytics

* Variety popularity analysis
* Revenue estimation
* Location-based analysis
* Price variation analysis
* Correlation analysis

### 3. Machine Learning

Two classification models are developed to predict high-revenue listings:

* Logistic Regression (baseline model)
* Random Forest (machine learning model)

Model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score

### 4. Explainable AI

SHAP (SHapley Additive exPlanations) is used to identify the most influential factors associated with high-revenue Hoya listings.

## Preliminary Findings

* Several Hoya varieties dominate marketplace activity.
* Price, customer reviews, and ratings are important predictors of listing performance.
* Random Forest outperforms Logistic Regression in classifying high-revenue listings.
* SHAP analysis provides interpretable insights into marketplace success factors.

## Conference Submission

This project is being prepared for submission to IC3INA 2026 under the track:

**Computational Systems and Data-Driven Engineering Applications**

with emphasis on:

* Machine Learning and AI Systems
* Explainable Artificial Intelligence (XAI)
* Data-Driven Decision Support Systems

## Author

Firila Najma Wahidah

Department of Statistics
The University of British Columbia