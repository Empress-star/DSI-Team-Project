# DSI Cohort 6 Team Project - Customer Purchasing Behaviours
**Project Status:** Active

## Project Intro / Objective

The purpose of this project is to create customer personas by identifying groups of customers with similar demographic and purchasing behaviour. We aim to leverage clustering and exploratory data analysis to better understand customer segments, uncover patterns in behaviour, and generate insights that can inform marketing decisions.

In modern marketing and customer relationship management, understanding purchasing behaviour is critical for driving business success. Companies across sectors — including retail, e-commerce, financial services, and telecommunications — use customer segmentation to tailor campaigns, personalize offers, and optimize product development.

This project mirrors real-world data science applications in:
    - Customer segmentation for targeted marketing strategies
    - Churn prediction and retention planning
    - Product recommendation systems
    - Personalized communications and campaign optimization

By identifying actionable customer personas, businesses can better allocate marketing budgets, increase customer lifetime value (CLV), and improve overall customer experience. Our approach aligns with industry practices such as RFM (Recency, Frequency, Monetary) analysis and clustering models frequently used in CRM and BI platforms.

## Members

- Adriana Meraz
- Carolina Crespo
- Mubashara Malbari
- Ryan O'Grady
- Scott Lewis
- Surbhi Maheshwari
- Ts'ui Toy

## Project Question

- Can we use existing customer data to identify distinct customer clusters based on their purchasing behavior and demographic characteristics?


## Project Description

We are working with a structured dataset of customer transactions and demographics. Our goal is to:

- Understand the key features driving purchasing behaviours
- Create customer segments using clustering techniques
- Explore how demographics correlate with spending habits
- Present actionable personas and recommendations based on these insights

## Dataset Overview

- Source: Kaggle ([link](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis?resource=download))
- Records: ~2,200 customers
- Features: 29 variables including demographics, spending habits, and campaign response

## Key Features:

- Demographics: Age, Education, Marital_Status, Income, Children, etc.
- Purchases: Amount spent on products such as wine, fruits, meat, fish, etc.
- Engagement: Number of store visits, campaign responses, online purchases
- RFM Variables: Recency (last purchase in days), Frequency, and Monetary metrics derived


## Methods Used:

- Data Cleaning and Pre-Analysis
    - We performed several steps to clean and prepare the data:
        - Removed null values and duplicates
        - Combined related features (e.g., total spending)
        - Normalized skewed distributions
        - Converted categorical features into numeric representations (One-Hot Encoding or Label Encoding)
        - Created new features like Age, Total Spending, Family Size, etc.
        - Scaled data using MinMaxScaler for clustering

- Exploratory Data Analysis 
    - Our EDA focused on uncovering patterns in:
        - Spending habits by age and income
        - Correlation between family size and product category preferences
        - Customer engagement across marketing channels
        - Campaign effectiveness by segment
    - We used heatmaps, histograms, boxplots, pairplots, and bar charts to visualize relationships and trends.

- Clustering (K-Means)
    - We applied K-Means Clustering after standardizing and transforming the features. The optimal number of clusters was determined using:
        - Elbow Method

- Data Visualization For Person Storytelling
    - We identified 3 distinct customer personas based on clustering analysis:
        - 1. Budget-Conscious Families (Cluster 0)

            - Low income (~$35K) and low spending (~$97)
            - Average age (~53), with ~1.2 children
            - Low purchase volume across all categories
            - Prefer in-store shopping, with low campaign engagement
        - 2. Mid-Income Traditional Shoppers (Cluster 1)

            - Moderate income (~$57K) and mid-level spending (~$730)
            - Older demographic (~59), mostly married
            - High purchases in wine and meat, moderate catalog/web use
            - Balanced cart size and channel usage
        - 3. Affluent Gourmet Enthusiasts (Cluster 2)

            - High income (~$76K) and highest spending (~$1,414)
            - Slightly younger (~56), but few or no children
            - Very high online engagement and luxury product interest (wine, meat, gold)
            - Highest cart size and purchase frequency


## Technologies Used

- Python
- Jupyter Notebooks
- Kagglehub
- Pandas, NumPy, scikit-learn, matplotlib

## Business Recommendations

Based on the insights from each persona, we recommend:

- Targeted Campaigns: Tailor discounts and offers by segment (e.g., luxury bundle for High-Income Gourmet)
- Channel Strategy: Increase digital marketing for tech-savvy young customers
- Customer Retention: Use RFM segmentation to re-engage dormant or low-frequency customers
- Product Development: Stock preferences based on cluster-specific demand (e.g., fish and fruit for older segments)


## Reproducibility

The reproducible part of this project is the entire Jupyter Notebook. 

## How to Run the Project

### Requirements
- Python 3.9+
- Jupyter Notebooks
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## Getting Started

1. Clone this repo: https://github.com/Empress-star/DSI-Team-Project.git
2. Install dependencies: pip install -r requirements.txt
3. Launch Jupyter Notebook and run: jupyter notebook
4. Open customer_segmentation.ipynb and run all cells.


## Folder Structure

DSI-Team-Project/
│
├── dataset/
│   └── marketing_campaign.csv
│
├── Visualizations/
│   └── visuals.png
│
├── DS5_Team_Project.ipynb/
│   
│
├── README.md


## References

- Kaggle Dataset: Customer Personality Analysis
- "Data Science for Business" by Provost & Fawcett
- scikit-learn documentation
- https://youtu.be/FM4YiiQNds4

