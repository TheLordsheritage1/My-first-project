# DSA- Data Documentation using MS Excel.
This was where I was able to attempt my very first project as a data analyst.

## Table of contents 
 - Project topic.
 - Project overview.
 - Tools used
 - Dataset description.
 - Data cleaning and preparation.
 - exploratory data analysis.
 - challenges.
 - conclusion 

# Project topic: Amazon product review analysis.

## Product overview
 This data analysis project provides a comprehensive insights on key trends, customer's prefernces and product performance of retail tech, a company which provides e-commerce to sellers on platforms like amazon over the past years. 
By leveraging, cleaning, exploration and visualization techniques this project will be able to give insightful key findings on how businesses can understand consumer behavior, initiate customer engagement and improve product strategy.

 The analysis covers rating distribution,total revenue,rating count,discount impact based on combined review metrics. 
The analysis process encompasses different stages:data source, data set description,data cleaning and preparation,tools used, exploratory data analysis, challenges, conclusion.

## Tools Used
- Microsoft excel[download here](https://www.microsoft.com)
  - for initial data exploration.
  - for data cleaning.
  - for data filtering.
  - for pivit table analysis.
 
## Data set description 
  a. **Data source**

The primary source of data used for this project was provided as part of a stuctured assignment. It contains data from retail tech and was used for academic and analytical purpose.

  b. **Key fields**
 
 The data set contains approximately 1466 rows and 16 columns. The data set captures customers feedback on a wide range of products and some of the key columns include
 - product id: this is a unique identifier for each product
 - product name: The name or title of the product reviewed.
 - user id: unique identifier of the customer who submitted the reviw.
 - category: this is the classification or the type of product
 - rating: this is the star rating provided by the customer(usually from 1-5)
 - actual proce: this is the original amount of products before any discount is given.
 - rating count: this is the total number of ratings received by a product.
 - discount percentage: this is the portion by which the original price of a product has already been reduced

  Some entrues included missing figures or inconsistent values especially in the rating, actual price and rating count but was handled and corrected during the data cleaning process.

## Data cleaning and preparation 
 Before any analysis was conducted, a comprehensive cleaning and preparation process was conduction. This step was essential for transforming the raw data into a structured and analysis-ready format. Several quality checks and process techniques were applied to preprocessing techniques to address missing values, eliminate redundancies, correct data types, and standardize entries across key fields.
The following steps taken were:

1. Data loading and inspection:
The data was first loaded and inspected to detect or identify any missing value or any sort of error that needs correction 
  
3. Handling Missing Values:
We identified and addressed missing values in key columns such as Ratings and Rating Count.
Missing Discount values were replaced with 0, assuming no discount was applied.

3. Removing Duplicates:
Duplicate entries were removed based on User ID, Product ID, and Review Content to eliminate repetition and ensure unbiased results.

4. Correcting Data Types:
Several columns were converted, columns like Rating, Actual Price, and Discounted Price e.t.c to numerical types where necessary and verified that text columns such as Product Name and Review were in the correct string format.

5. Standardization:
Some columns were standardized for effective application and consistency. E.g The product name was changed to “new product name” as the former was too long and had to be trimmed. Some columns had unwanted characters in text columns and this had to be removed.

6. Final Checks:
The data set was confirmed to be free of null values, unnecessary duplicates, and formatting issues. It was also ensured that all fields were ready for analysis and visualization.
Below is the before and after view of the data set. 

## Exploratory Data Analysis (EDA)

### Overview
  The Exploratory Data Analysis (EDA) phase was conducted to understand the underlying structure of the dataset, identify key patterns, spot anomalies, and extract meaningful relationships between variables. Some of the questions asked and answered was:

#### a. *What is the total number of reviews per category?*

 To determine the total number of reviews per category, the rating count column was summed up under the pivot table and the data was grouped by category.

 This shows that electronic products have the highest review either due to customer's interest in the product or the quality of such product. This may help in prioritizing product improvement and company resources.

#### b. *Which product has the highest average rating?*

 To arrive at this I used the excel function “average” to get the average of the rating, then I sorted the data to reveal the top 10 products with the highest rating and I grouped the data under product Id.

  The ratings ranged from 1 to 5, with the majority of the top products receiving between 4 to 5 stars. This indicates a generally positive customer experience.

#### c. *What is the average actual price vs the discounted price by category?*

 To understand the pricing dynamics across different product categories, I computed the average actual price and the average discount price for each category. This comparison highlights how much, on average, customers are expected to pay versus the discounted amounts offered.

 This concludes that pricing patterns may influence purchasing behavior and customer preferences within each category.

#### d. *What is the number of unique products per price range bucket?*

  A price range bucket is a way to group products or items into categories based on their prices. Instead of listing every exact price,it assists in analyzing products more easily 
 To gain insight into the distribution of products across different pricing levels, I grouped the data into 3 different price range buckets(<200, 200-500, >500). How I did that was I created a new or calculated column, named it “Price bucket” and used the excel formula to segment the actual price into defined ranges and then counted the number of unique products within each bucket.
I also grouped the new product name and set it to a distinct count.

The result of this analysis helps us understand whether most products are concentrated in low-price or high-price categories, which is valuable for pricing strategies and inventory planning.

#### e. *What is the potential revenue by category?*

To calculate how much revenue each product category could generate, the method used to derive a potential revenue column was to create a calculated column using excel formula(=actual price * rating count).This assumes each rating represents a unit sold. The results were then grouped by category to identify which categories have the highest revenue potential.

From the analysis, categories like Electronics and computer& accessories showed the highest potential revenue, indicating strong customer engagement and higher-value products.






