# PRODIGY_ML_02
# Mall Customer Segmentation using K-Means Clustering

This project performs customer segmentation using K-Means clustering on retail customer data to identify distinct groups based on demographic and spending characteristics.

## 📁 Files in this Repository
- `task2_code.ipynb` –Jupyter notebook containing:
  - Data loading and preprocessing
  - Exploratory Data Analysis (EDA)
  - K-Means clustering implementation
  - Visualization of results
  - Business interpretation
- `task2_data.xlsx` –Original dataset containing:
  - Customer demographics (Age, Gender)
  - Financial features (Annual Income)
  - Behavioral metric (Spending Score)
- `/images` – Directory containing visualizations:
  - `elbow_method.png` 
  - `cluster_visualization.png` 
- 
## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Dataset](#dataset)
- [Methodology](#methodology)


## Project Overview
This analysis helps retailers:
- Identify distinct customer segments
- Understand spending patterns
- Develop targeted marketing strategies
- Optimize product offerings
- Improve customer engagement

## Key Features
- Data preprocessing and normalization
- Optimal cluster determination using:
  - Elbow Method
  - Silhouette Analysis
- K-Means clustering implementation
- Interactive visualization of clusters
- Detailed business interpretation


## Dataset Description
The dataset `task2_data.xlsx` contains:
- **200 records** of customer information
- **Key Features**:
  - `CustomerID`: Unique identifier
  - `Gender`: Male/Female
  - `Age`: Customer age
  - `Annual Income (k$)`: Yearly income in thousands
  - `Spending Score (1-100)`: Customer spending rating

**Sample Data**:
| CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100) |
|------------|--------|-----|--------------------|------------------------|
| 1          | Male   | 19  | 15                 | 39                     |
| 2          | Male   | 21  | 15                 | 81                     |


## Methodology
1. **Data Preparation**:
   - Loaded and cleaned the dataset
   - Selected relevant features (Age, Annual Income, Spending Score)
   - Standardized features using StandardScaler

2. **Cluster Analysis**:
   - Determined optimal clusters (k=5) using:
     - Elbow Method (WCSS)
     - Silhouette Score
   - Applied K-Means++ algorithm

3. **Visualization**:
   - 2D and 3D cluster plots
   - Feature distribution analysis
   - Cluster centroid analysis

4. **Interpretation**:
   - Analyzed cluster characteristics
   - Developed customer personas

## Results
The analysis identified 5 distinct customer segments:

| Cluster | Age Range | Income Level | Spending Level | Segment Name          |
|---------|-----------|--------------|----------------|-----------------------|
| 0       | 20-35     | Medium       | High           | Young Spenders        |
| 1       | 25-40     | High         | Medium         | Career Professionals  |
| 2       | 40-60     | Low          | Low            | Conservative Seniors  |
| 3       | 18-25     | Low          | High           | Budget-Conscious Youth|
| 4       | 30-50     | High         | High           | Affluent Shoppers     |






