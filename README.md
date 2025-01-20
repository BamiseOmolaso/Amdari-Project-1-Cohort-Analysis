# Amdari Project 1: Cohort Analysis and Customer Segmentation using Kmeans

This repository contains the implementation of a **Cohort Analysis and Customer Segmentation** project for an e-commerce company. The project focuses on understanding customer behavior, retention patterns, and segmentation using clustering techniques.

## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Analysis Steps](#analysis-steps)
- [Key Insights](#key-insights)
- [Technologies Used](#technologies-used)
- [How to Use](#how-to-use)
- [Results](#results)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Project Overview
E-commerce companies often face challenges in retaining customers and improving their shopping experiences. This project leverages **Cohort Analysis** and **K-Means Clustering** to:

- Analyze customer retention rates.
- Identify purchasing patterns.
- Segment customers into meaningful groups to enable targeted marketing strategies.

This project was conducted using Python and explores key metrics such as recency, frequency, and monetary value (RFM).

## Objectives
The key objectives of this project are:
1. Perform a retention-based cohort analysis to track customer behavior over time.
2. Segment customers into clusters using K-Means clustering based on purchasing patterns.
3. Derive actionable insights to improve customer retention and loyalty.

## Dataset Description
The dataset includes the following fields:

| Column       | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| InvoiceNo    | Unique identifier for each invoice or transaction.                         |
| InvoiceDate  | Date and time of the transaction.                                           |
| CustomerID   | Unique identifier for each customer.                                        |
| StockCode    | Code for specific products in the inventory.                                |
| Description  | Description of the purchased product.                                       |
| Quantity     | Number of units purchased in the transaction.                               |
| UnitPrice    | Price per unit of the product.                                              |
| Country      | Country where the transaction took place.                                   |

## Analysis Steps
1. **Data Preprocessing**:
    - Handle missing values.
    - Clean and transform data for analysis.
    - Extract cohort dates and calculate cohort indices.

2. **Cohort Analysis**:
    - Group customers by their first purchase date (cohort date).
    - Analyze retention rates over time.

3. **Feature Engineering**:
    - Create aggregated features such as recency, quantity, and average unit price for each customer.

4. **Clustering**:
    - Apply K-Means clustering to segment customers based on purchasing patterns.
    - Use the Elbow Method to determine the optimal number of clusters.

5. **Insights Extraction**:
    - Analyze top products and countries for each cluster.
    - Generate actionable insights based on clustering results.

## Key Insights
1. Customers were segmented into 3 clusters based on recency, quantity, and spending patterns:
   - **Cluster 0**: Customers with moderate purchases and less frequent activity.
   - **Cluster 1**: Highly engaged customers with frequent and high-value purchases.
   - **Cluster 2**: Recently active customers with relatively low purchase volumes.

2. Top products and countries for each cluster were identified to guide targeted marketing efforts.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Tools**: Jupyter Notebook, Google Colab, Git

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/BamiseOmolaso/Amdari-Project-1-Cohort-Analysis.git
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:
   ```bash
   https://github.com/BamiseOmolaso/Amdari-Project-1-Cohort-Analysis/blob/main/cohort_analysis_solution.ipynb
   ```

4. Follow the notebook to reproduce the analysis and explore the insights.

## Results
- **Retention Rates**: Cohort analysis revealed the drop-off points in customer retention, enabling the company to focus on these critical timeframes.
- **Customer Segments**: Clustering highlighted three distinct customer groups, providing valuable input for personalized marketing strategies.
- **Product Trends**: Popular products and countries for each cluster were identified to optimize inventory and marketing efforts.

## Future Work
- Integrate the findings into a recommendation engine for personalized product suggestions.
- Expand clustering analysis to include more features like geographic location and product categories.
- Explore advanced models such as DBSCAN or hierarchical clustering for better segmentation.

## Contributors
This project was an improvement on the Amdari Cohort Analysis guide by:
- **[Bamise Omolaso](https://github.com/BamiseOmolaso)**
