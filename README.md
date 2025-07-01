# DSA-Project 1

This is my first portfolio project, created as part of my learning journey at the Incubator Hub.  
Through the Data Analysis track, I’ve gained practical experience using Microsoft Excel, SQL, and Power BI to explore and visualize real-world data.

## Table of Contents
- [Project Topic](#project-topic)
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning](#data-cleaning)
- [Explanatory Data Analysis](#explanatory-data-analysis)
- [Data Analysis](#data-analysis)
- [My Analysis](#my-analysis)
- [Conclusion](#conclusion)
- [Next Steps](#next-steps)
- [Feedback](#feedback)

## Project Topic
**Amazon Product Review Analysis**

## Project Overview
This project is a comprehensive Excel-based analysis of Amazon product data, covering pricing patterns, discount distribution, customer reviews, and category-level metrics.  
It includes pivot tables, calculated columns, and an interactive dashboard for actionable business insights.

## Data Source
The dataset contains information scraped from Amazon product pages.

## Tools Used
- Microsoft Excel (Pivot Tables, Charts, Calculated Fields) – [Download here](https://www.microsoft.com)
  - For data collection
  - For data cleaning
  - For dashboard design and layout

## Data Cleaning
In the cleaning process, I began with a thorough check of the raw dataset to identify issues such as:
1. Missing values and blank cells  
2. Irrelevant columns

## Explanatory Data Analysis
EDA involved answering key questions about the dataset to uncover trends, patterns, and relationships. These questions included:

1. What is the average discount percentage by product category?  
2. How many products are listed under each category?  
3. What is the total number of reviews per category?  
4. Which products have the highest average ratings?  
5. What is the average actual price vs discounted price by category?  
6. Which products have the highest number of reviews?  
7. How many products have a discount of 50% or more?  
8. What is the distribution of product ratings (e.g., how many are rated 3.0, 4.0, etc.)?  
9. What is the total potential revenue (actual_price × rating_count) by category?  
10. What is the number of unique products per price range bucket: `<₹200`, `₹200–₹500`, `>₹500`?  
11. How does the rating relate to discount level?  
12. How many products have fewer than 1,000 reviews?  
13. Which categories have products with the highest discounts?  
14. Identify the top 5 products based on a combination of rating and review count.

## Data Analysis
This section outlines some of the key queries and functions applied during the analysis phase:

- `IF` – for creating price range buckets and filtering conditions  
- `AVERAGE` – to compute average ratings, discounts, and prices  
- `COUNT` – for counting reviews  
- Pivot Tables – for category summaries, rating distributions, and top products  
- **Calculated Fields**:
  - `discount_percentage = (actual - discounted)/actual * 100`
  - `potential_revenue = actual_price × rating_count`
  - `price_bucket = IF(price < 200, ..., ...)`

## My Analysis
- The majority of the products are priced over ₹500  
- Electronics and Computer Accessories have the highest potential revenue, discounts, and review volumes  
- Only a few categories (Electronics, Computer Accessories, and Home & Kitchen) contribute most of the revenue, while the majority contribute far less  
- Higher discounts do not necessarily lead to higher ratings

## My Recommendation
This project helped me develop practical skills in data cleaning, analysis, and visualization using Excel. I discovered how to interpret raw product data and convert it into meaningful business insights.  
A key takeaway is that adiscounting does not automatically improve customer satisfaction or product ratings, businesses should evaluate multiple factors when optimizing product strategies.















   





     
