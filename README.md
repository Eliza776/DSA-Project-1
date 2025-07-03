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

![image](https://github.com/user-attachments/assets/fa7cd278-9a88-40f3-af88-241c2a490408)

 -Pivot Table

 AVERAGE DISCOUNT PERCENTAGE BY CATEGORY	
Row Labels	Average of discount_percentage
Car&Motorbike	42%
Computers&Accessories	54%
Electronics	51%
Health&PersonalCare	53%
Home&Kitchen	40%
HomeImprovement	58%
MusicalInstruments	46%
OfficeProducts	12%
Toys&Games	0%
Grand Total	48%
![image](https://github.com/user-attachments/assets/7af67e1e-7bc7-475e-add7-a5432ebd9c33)

NUMBER OF PRODUCTS PER CATEGORY	
Row Labels	Count of product_id
Car&Motorbike	1
Computers&Accessories	453
Electronics	526
Health&PersonalCare	1
Home&Kitchen	448
HomeImprovement	2
MusicalInstruments	2
OfficeProducts	31
Toys&Games	1
Grand Total	1465
![image](https://github.com/user-attachments/assets/b2ba663a-ada7-4c8b-b805-3949d4d6c374)

AVERAGE ACTUAL PRICE VS DISCOUNTED PRICE BY CATEGORY		
Row Labels	Average of discounted_price	Average of actual_price
Car&Motorbike	₹ 2,339.00	₹ 4,000.00
Computers&Accessories	₹ 842.65	₹ 1,683.62
Electronics	₹ 5,965.89	₹ 10,127.31
Health&PersonalCare	₹ 899.00	₹ 1,900.00
Home&Kitchen	₹ 2,330.62	₹ 4,162.07
HomeImprovement	₹ 337.00	₹ 799.00
MusicalInstruments	₹ 638.00	₹ 1,347.00
OfficeProducts	₹ 301.58	₹ 397.19
Toys&Games	₹ 150.00	₹ 150.00
Grand Total	₹ 3,125.31	₹ 5,444.99
![image](https://github.com/user-attachments/assets/60b153d3-e0a8-4488-a9b4-7733135dc991)

TOTAL NUMBER OF REVIEWS PER CATEGORY	
Row Labels	Sum of rating_count
Car&Motorbike	1,118.00
Computers&Accessories	7,728,689.00
Electronics	15,778,848.00
Health&PersonalCare	3,663.00
Home&Kitchen	2,991,069.00
HomeImprovement	8,566.00
MusicalInstruments	88,882.00
OfficeProducts	149,675.00
Toys&Games	15,867.00
Grand Total	26,766,377.00
![image](https://github.com/user-attachments/assets/9bebdf8c-9dba-4637-8e28-e765bbd131f9)

TOP 10 PRODUCTS WITH THE HIGESHT NUMBER OF REVIEWS	
Row Labels	Sum of rating_count
boAt	4,445,359.00
AmazonBasics	2,034,664.00
Redmi	1,878,482.00
SanDisk	1,426,074.00
TP-Link	1,354,798.00
Amazon	1,207,959.00
MI	1,069,730.00
Samsung	901,882.00
JBL	891,075.00
Noise	621,421.00
Grand Total	15,831,444.00
![image](https://github.com/user-attachments/assets/5dc44845-d2ac-4a25-a9f0-914a8a945911)

PRODUCT COUNT WITH <1000 REVIEWS	
Row Labels	Count of product_id
No	328
Yes	1137
Grand Total	1465
![image](https://github.com/user-attachments/assets/8ef2771f-414d-4c7c-ac38-749b6d4a91fd)

TOP 5 PRODUTS BY RATING AND REVIEWS COMBINED	
Row Labels	Sum of Rating +Review Composite
boAt	4723.16
AmazonBasics	2198.36
Redmi	1983.88
SanDisk	1500.37
TP-Link	1441.00
Grand Total	11846.78
![image](https://github.com/user-attachments/assets/00538cc1-4995-448d-a0d9-ae64fab4219b)


TOTAL POTENTIAL REVENUE	
Row Labels	Sum of Total potential revenue
Car&Motorbike	₹ 4,472,000.00
Computers&Accessories	₹ 12,614,826,243.00
Electronics	₹ 98,020,806,794.00
Health&PersonalCare	₹ 6,959,700.00
Home&Kitchen	₹ 10,459,722,337.00
HomeImprovement	₹ 6,163,434.00
MusicalInstruments	₹ 151,117,062.00
OfficeProducts	₹ 60,778,817.00
Toys&Games	₹ 2,380,050.00
Grand Total	₹ 121,327,226,437.00
![image](https://github.com/user-attachments/assets/a40ed739-606e-4c30-9724-331eb8be651e)

CATEGORIES WITH HIGHEST DISCOUNT	
Row Labels	Max of discount_percentage
Computers&Accessories	94%
Electronics	91%
Home&Kitchen	90%
OfficeProducts	75%
MusicalInstruments	60%
HomeImprovement	58%
Health&PersonalCare	53%
Car&Motorbike	42%
Toys&Games	0%
Grand Total	94%
![image](https://github.com/user-attachments/assets/1320221c-e4b6-4253-a9c9-911c44a03456)


TOP 5 PRODUTS BY RATING AND REVIEWS COMBINED	
Row Labels	Sum of Rating +Review Composite
boAt	4723.16
AmazonBasics	2198.36
Redmi	1983.88
SanDisk	1500.37
TP-Link	1441.00
Grand Total	11846.78
![image](https://github.com/user-attachments/assets/1174481f-244f-44dd-903b-77f5655f4d2e)

TOP 10 PRODUCTS WITH THE HIGHEST AVERAGE RATINGS	
Row Labels	Average of rating
REDTECH	5.00
Syncwire	5.00
Swiffer	4.80
Oratech	4.80
Instant	4.80
Multifunctional	4.70
FIGMENT	4.70
Campfire	4.70
Aquadpure	4.60
VRPRIME	4.60
10k	4.60
Melbon	4.60
Grand Total	4.74
![image](https://github.com/user-attachments/assets/c072bb91-6030-4545-98cd-575589c655f4)

PRICE RANGE BUCKET	
Row Labels	Count of Product Name
₹200 - ₹500	183
<₹200	37
>₹500	1245
Grand Total	1465
![image](https://github.com/user-attachments/assets/e96f1af6-a309-44ed-9c97-2127d58e2103)

DISCOUNT RANGE	
Row Labels	Count of Product Name
50% or more	751
less than 50%	714
Grand Total	1465
![image](https://github.com/user-attachments/assets/17520ca0-b9e1-4dd3-a15c-15cc54d247f8)


PRODUCT RATING DISTRIBUTION	
Row Labels	Count of Product Name
0	1
2	2
3	40
4	1318
5	104
Grand Total	1465
![image](https://github.com/user-attachments/assets/d75f62dc-168d-4229-a7cf-5f79c1e6eb02)


RATINGS IN RELATION TO DISCOUNT BUCKET	
Row Labels	Average of rating
0-10%	4.21
11-20%	4.14
21-30%	4.15
31-40%	4.10
41-50%	4.10
51-60%	4.06
61-70%	4.11
71-80%	4.03
81-90%	3.95
91-100%	4.22
Grand Total	4.10
	
![image](https://github.com/user-attachments/assets/a25f8637-90bd-472a-b930-c3dd6d99df0b)
























  
## My Recommendation
This project helped me develop practical skills in data cleaning, analysis, and visualization using Excel. I discovered how to interpret raw product data and convert it into meaningful business insights.  
My key takeaways are ;
-The business should invest more in Electronics and Computer Accessories as they show the highest revenue potential.
- High discounts (91–100%) are associated with higher ratings, the business should consider offering limited-time high discounts to boost product visibility and customer reviews especially for products generating less revenue.


















   





     
