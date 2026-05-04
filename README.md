# Wholesale Customer Segmentation using Clustering

## Overview

This project applies clustering techniques to segment wholesale customers based on their purchasing patterns.

The goal is to identify natural customer groups and generate insights that can support marketing, inventory planning, and customer management strategies.

This project was completed as part of the Statistical Modeling and Inferencing course at BITS Pilani.

---

## Problem Statement

Wholesale businesses serve different types of customers such as small shops, restaurants, and large distributors.

Using a single approach for all customers can lead to inefficiencies in:
- marketing
- inventory planning
- customer engagement

This project aims to identify distinct customer segments based on their purchasing behaviour.

---

## Dataset

The dataset used is the Wholesale Customers Dataset from UCI Machine Learning Repository.

It contains spending data across categories:

- Fresh
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicassen

Dataset link:

https://archive.ics.uci.edu/ml/machine-learning-databases/00292/Wholesale%20customers%20data.csv

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Approach

### Data Exploration
- checked distributions
- identified skewness
- analysed correlations
- visualised using histograms and heatmaps

### Data Preparation
- no missing values
- outliers retained as they represent real high-value customers
- features scaled using standardization

### Model Development
- applied K-Means clustering
- tested multiple values of K
- used Elbow Method and Silhouette Score

### Model Selection
- K = 3 selected
- best balance of interpretability and clustering quality

---

## Key Results

Three customer segments were identified:

### Cluster 1 – Regular Customers
- majority group
- moderate spending across categories

### Cluster 0 – High Grocery/Milk Buyers
- high spending on essential items
- likely retail or restaurant customers

### Cluster 2 – Extremely High Spenders
- very small group
- extremely high volume purchases
- likely large distributors

---

## Key Insights

- customer behaviour is not uniform
- Grocery, Milk, and Detergents drive segmentation strongly
- a small number of customers contribute very high volume
- most customers belong to a moderate spending group

---

## Business Recommendations

- design different strategies for each segment
- offer bulk discounts to high-volume customers
- create loyalty programs for regular customers
- treat extreme high spenders as strategic accounts

---

## Why This Project Matters

This project demonstrates how clustering techniques can uncover hidden patterns in customer behaviour.

It shows how statistical modeling can directly support business decisions in segmentation and targeting.

---

## Repository Structure
wholesale-customer-segmentation-clustering/

├── README.md
├── src/
│ └── wholesale_segmentation_clustering.py


---

## How to Run

Clone repository:
git clone https://github.com/chetanpant/wholesale-customer-segmentation-clustering.git


Install dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn


Run:
python src/wholesale_segmentation_clustering.py


---

## Project Context

This project was completed as part of the Statistical Modeling and Inferencing course.

It includes:
- data exploration
- clustering analysis
- model validation
- interpretation and insights
