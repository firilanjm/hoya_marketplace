# Hoya Marketplace Analytics and Explainable Machine Learning

This repository contains the data processing, exploratory analysis, and machine learning workflows used to assess the economic potential of Hoya ornamental plant trade in Indonesia using Shopee marketplace data.

## Project Overview

The study investigates marketplace activity related to Hoya ornamental plants by analyzing product listings collected from Shopee. The project combines descriptive marketplace analytics with explainable machine learning to identify factors associated with economically successful product listings.

The analysis focuses on:

* Hoya variety distribution
* Product pricing characteristics
* Seller geographic distribution
* Estimated marketplace revenue
* Correlation among marketplace indicators
* High-revenue listing classification using Random Forest
* Model interpretation using SHAP (SHapley Additive exPlanations)

## Dataset

The dataset consists of approximately 420 Hoya product listings collected from Shopee.

### Variables

| Variable          | Description                |
| ----------------- | -------------------------- |
| product_name      | Product title              |
| variety           | Hoya variety               |
| price             | Product price (IDR)        |
| number_sold       | Number of units sold       |
| location          | Seller location            |
| rating            | Product rating             |
| number_of_reviews | Number of customer reviews |
| marketplace       | Marketplace source         |
| scraping_date     | Date of data collection    |
| product_url       | Product URL                |
| shop_name         | Seller name                |

## Research Objectives

1. Analyze marketplace characteristics of Hoya ornamental plant trade.
2. Estimate the economic potential of Hoya trade using marketplace data.
3. Identify factors associated with high-revenue listings using explainable machine learning.

## Methodology

### Data Preparation

* Data cleaning and preprocessing
* Duplicate removal
* Numeric conversion of price and sales variables
* Standardization of variety names
* Removal of unidentified varieties for machine learning analysis

### Economic Potential Assessment

Estimated revenue was calculated as:

Revenue = Price × Number Sold

This metric represents cumulative estimated revenue based on publicly available marketplace information.

### Descriptive Analysis

* Variety frequency analysis
* Geographic distribution analysis
* Revenue analysis
* Correlation analysis

### Machine Learning

#### Random Forest Classification

A Random Forest classifier was developed to distinguish between:

* High-revenue listings
* Low-revenue listings

using marketplace attributes such as:

* Price
* Rating
* Number of reviews
* Variety
* Seller location

#### Explainability

SHAP (SHapley Additive exPlanations) was applied to identify the most influential predictors of marketplace success.

## Results Summary

### Random Forest Performance

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 80.3% |
| Precision | 89.3% |
| Recall    | 67.6% |
| F1-score  | 76.9% |

### Key Predictors

The most influential factors associated with high-revenue listings were:

1. Product price
2. Product rating
3. Number of reviews
4. Hoya variety
5. Seller location

## Conference Submission

This work is being prepared for submission to:

**The International Conference on Computer, Control, Informatics and its Applications (IC3INA 2026)**

Track:

* Machine Learning and AI Systems
* Decision-Support Systems for Engineering Applications

## Author

Firila Najma Wahidah

Department of Statistics
The University of British Columbia
Vancouver, Canada

## License

This repository is intended for academic and research purposes.
