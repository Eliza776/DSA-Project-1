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
- [My Recommendation](#my-recommendation)
  

## Project Topic
Amazon Product Review Analysis               

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
- Majority of the products are priced over ₹500  
- Electronics and Computer Accessories have the highest potential revenue, discounts, and review volumes
- A significant number of products (1,137) have fewer than 1,000 reviews, indicating many products lack customer engagement
- Majority of products are rated 4 stars (1,318) and 5 stars (104).
- Only a few categories (Electronics, Computer Accessories, and Home & Kitchen) contribute most of the revenue, while the majority contribute far less  
- Higher discounts can potentially lead to higher ratings and generate more revenue


![image](https://github.com/user-attachments/assets/d2caa229-15e7-461c-a891-9d1c84b8735c)

 ![image](https://github.com/user-attachments/assets/8f5dfa13-e8d7-4ed7-ba4f-44e7c9d22899)
 
![image](https://github.com/user-attachments/assets/4bea0d9e-39b3-4d98-ba84-cf5c1be1e2c3)

![image](https://github.com/user-attachments/assets/b6643faf-7054-458b-a97d-9fa60ff24db9)

![image](https://github.com/user-attachments/assets/bc3701ea-d491-4a92-8cc4-40c61f22ea48)

![image](https://github.com/user-attachments/assets/315d3380-e546-44d5-a42f-fd1ec570c767)

![image](https://github.com/user-attachments/assets/f8e38cd5-fbaa-4638-b29b-ac6dd4861268)

![image](https://github.com/user-attachments/assets/2a66bd35-5c2e-49fa-b833-a207535930c2)

![image](https://github.com/user-attachments/assets/3f71e864-4971-471f-af2f-ce74645e46f5)

![image](https://github.com/user-attachments/assets/c58b7610-5e82-46a2-a8a1-fdb9af80f5bf)

![image](https://github.com/user-attachments/assets/359f58a4-112a-4313-b8cc-8a359cfccc15)

![image](https://github.com/user-attachments/assets/6740e921-786c-463d-a4e5-4ae2cd762d76)

![image](https://github.com/user-attachments/assets/4024a8c8-f1e3-4116-9dea-778b9e3e9552)

![image](https://github.com/user-attachments/assets/f0016cf6-785e-4c14-b2be-e43f050fc75c)




Pivot Table

![image](https://github.com/user-attachments/assets/7af67e1e-7bc7-475e-add7-a5432ebd9c33)

![image](https://github.com/user-attachments/assets/b2ba663a-ada7-4c8b-b805-3949d4d6c374)


![image](https://github.com/user-attachments/assets/60b153d3-e0a8-4488-a9b4-7733135dc991)


![image](https://github.com/user-attachments/assets/9bebdf8c-9dba-4637-8e28-e765bbd131f9)


![image](https://github.com/user-attachments/assets/5dc44845-d2ac-4a25-a9f0-914a8a945911)


![image](https://github.com/user-attachments/assets/8ef2771f-414d-4c7c-ac38-749b6d4a91fd)


![image](https://github.com/user-attachments/assets/a40ed739-606e-4c30-9724-331eb8be651e)


![image](https://github.com/user-attachments/assets/1320221c-e4b6-4253-a9c9-911c44a03456)



![image](https://github.com/user-attachments/assets/1174481f-244f-44dd-903b-77f5655f4d2e)


![image](https://github.com/user-attachments/assets/c072bb91-6030-4545-98cd-575589c655f4)


![image](https://github.com/user-attachments/assets/e96f1af6-a309-44ed-9c97-2127d58e2103)


![image](https://github.com/user-attachments/assets/17520ca0-b9e1-4dd3-a15c-15cc54d247f8)



![image](https://github.com/user-attachments/assets/d75f62dc-168d-4229-a7cf-5f79c1e6eb02)


	
![image](https://github.com/user-attachments/assets/a25f8637-90bd-472a-b930-c3dd6d99df0b)




  
## My Recommendation
This project helped me develop practical skills in data cleaning, analysis, and visualization using Excel. I discovered how to interpret raw product data and convert it into meaningful business insights.  
My key takeaways are ;
-The business should invest more in Electronics and Computer Accessories as they show the highest revenue potential.
- High discounts (91–100%) are associated with higher ratings, the business should consider offering limited-time high discounts to boost product visibility and customer reviews especially for products generating less revenue.


















   





     
