# DSA- Data Documentation using MS Excel.
This was where I was able to attempt my very first project as a data analyst.

## Table of contents 
 - Project topic.
 - Project overview.
 - Data description
 - Data cleaning and preparation
 - Tools used
 - exploratory data analysis
 - challenges
 - conclusion 

# Project topic: Amazon product review analysis.

## Product overview
 This data analysis project provides a comprehensive insights on key trends, customer's prefernces and product performance of retail tech, a company which provides e-commerce to sellers on platforms like amazon over the past years. 
By leveraging, cleaning, exploration and visualization techniques this project will be able to give insightful key findings on how businesses can understand consumer behavior, initiate customer engagement and improve product strategy.

 The analysis covers rating distribution,total revenue,rating count,discount impact based on combined review metrics. 
The analysis process encompasses different stages:data source, data set description,data cleaning and preparation,tools used, exploratory data analysis, challenges, conclusion.

## Data set description 
 1 **Data source**
 The primary source of data used for this project was provided as part of a stuctured assignment. It contains data from retail tech and was used for academic and analytical purpose.

  2 **Features**
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

Data loading and inspection: The data was first loaded and inspected to detect or identify any missing value or any sort of error that needs correction 
  
Handling Missing Values:
We identified and addressed missing values in key columns such as Ratings and Rating Count.
Missing Discount values were replaced with 0, assuming no discount was applied.

 Removing Duplicates:
Duplicate entries were removed based on User ID, Product ID, and Review Content to eliminate repetition and ensure unbiased results.


Correcting Data Types
Several columns were converted, columns like Rating, Actual Price, and Discounted Price e.t.c to numerical types where necessary and verified that text columns such as Product Name and Review were in the correct string format.

Standardization:
Some columns were standardized for effective application and consistency. E.g The product name was changed to “new product name” as the former was too long and had to be trimmed. Some columns had unwanted characters in text columns and this had to be removed.


Final Checks:
The data set was confirmed to be free of null values, unnecessary duplicates, and formatting issues. It was also ensured that all fields were ready for analysis and visualization. 


