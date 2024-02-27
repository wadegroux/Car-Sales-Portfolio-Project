# Car Sales Data Analysis Project

![automobile-1291491_640](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/cdfa0bc2-f4c2-4b08-9bfa-b59c9c5c2a3c)

## Introduction
This data analysis project demonstrates my proficiency in extracting valuable insights from a comprehensive car sales dataset sourced from Kaggle. Similar to my prior work on US traffic accidents, where the dataset spanned from February 2016 to March 2023, the current analysis dives into the dynamic world of car sales. Through a combination of critical thinking, meticulous data cleaning, thorough analysis, and effective visualization, this project aims to uncover patterns and trends within the provided dataset.

## Problem Statement
In the realm of car sales, understanding the underlying factors that influence customer choices, dealer success, and market trends is paramount. The goal of this analysis is to extract actionable insights from the provided dataset, shedding light on critical aspects such as popular car models, customer demographics, and regional variations in sales. By addressing these key questions, we aim to empower stakeholders in the automotive industry to optimize marketing strategies, tailor inventory management, and enhance overall business performance.

## Objective
The primary objective of this data analysis project is to provide a comprehensive understanding of the car sales dataset and offer actionable insights for strategic decision-making in the competitive landscape of the automotive industry. This project showcases the application of critical data analysis skills and tools, including SQL for initial cleaning and Tableau for detailed visual analysis.

## Questions to be Answered
1. **Popular Car Models:** Which car models are the most popular in terms of sales volume, and what are their key characteristics?
2. **Demographic Analysis:** How does the distribution of annual income and gender vary among the customers purchasing cars? Are there any notable trends or preferences?
3. **Temporal Trends:** What are the monthly and yearly trends in car sales? Are there any seasonal patterns that can be identified?
4. **Dealer Performance:** Which dealerships exhibit the highest sales volume, and how does their performance vary across different regions?
5. **Regional Disparities:** Are there significant variations in car sales across different regions? What factors may contribute to these regional disparities?

Feel free to explore the project, review the analysis process, and contribute to further enhancements. Your insights and feedback are highly appreciated!

## Data Sourcing
The dataset utilized in this analysis project was sourced from Kaggle, a popular platform for datasets and data science competitions. Specifically, the dataset covers a comprehensive collection of car sales transactions and associated details. The original dataset, contributed by Kaggle user Vasu Avasthi, was obtained from Kaggle's dataset repository.

## Data Assessment
**Explore the Data:**

I will use the select statement to examine a sample of rows from each table. This will allow me to understand the data types, ranges, and overall structure of my data table. 

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/7fe916c5-1dcf-49b6-b633-6f2bc297ec0f)

From looking at this I can see that I have 16 unique columns that contain various unique values. I can see that I have the Date of purchase for each sale the region of the sale and the various information about the cars that were purchased.

**Check For Missing Values:**

Now I will Identify columns with missing values. I can do this by using 'COUNT' and 'IS NULL' Conditions to assess missing values.

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/b0777b17-75fe-48fd-b0ff-98fcf14cd399)

I did this for every column and there were no missing values

**Check for Duplicates** 

I will check for duplicatees to do this I need to identify duplicate rows in the dataset. Since column Car_id is a unique identifier for each row and should not have duplicate values I can use it to check for the presence of duplicate rows. 

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/7a5b512f-7778-4eb0-9929-7d477a082dc0)

As you can see there are no duplicated rows

## Data Cleaning

### Addressing Duplicate, Missing, or Null Data
Despite the cleanliness of the dataset, it's crucial to recognize that real-world data often presents challenges. In instances where duplicate, missing, or null data might be encountered, this assessment phase would typically be the stage to strategize and implement solutions. Common actions include:
- **Duplicate Data:** Identification and removal or consolidation based on business rules.
- **Missing or Null Data:** Decision on imputation methods, deletion, or acknowledgment in subsequent analysis.

Fortunately, the current dataset did not require such interventions, allowing for a streamlined transition to the subsequent phases of data exploration and analysis.

The absence of data quality issues during the assessment stage is a positive indicator, facilitating a more efficient and focused analysis process.

## Exploratory Data Analysis "EDA"
### Access Data Distribution 
I will write a query that will count the number of Unique Companies

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/e50357a4-eec0-4e9e-9e3c-072be44e0c0a)

There are 30 Different companies within the data table

**Colors:**
I will now write a query that shows how many different distinct colors there are in the dataset

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/d160233a-76c3-4fa6-baf5-22d00f802c1a)

There are only 3 unique color options for cars within the data table 

**Models and their Counts:**
I will write a query that will show me the unique models and how many of the sales are along with them

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/91344df3-7959-46b5-a216-de867763a4fe)

This allowed me to see that there are 154 different models and how many sales each of the models have

### Analyze Numerical Counts
**Summary Statistics for 'Price'**
I will get summary statistics for price by finding out the average price, the minimum prize and the max price 

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/63b0d6c9-6b5c-4787-b429-11d64f67ca79)

**Summary Statistics for 'Annual Income'**
I will also get the average min and max for the annual income column 

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/7519734e-469c-4bae-9bf7-0478f065a3f5)

### Identify Trends Overtime 
**Monthly Sales Count Over Time**

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/82dc76f4-39ee-4396-ad81-2eea43e85da5)

This query uses the YEAR(Date) and Month(DATE) to extract the year and month from the 'Date' Column

**Yearly Sales Count Over Time**

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/3bf5a98e-3fe4-4fef-916a-319a7977a2b9)

This shows me that 2023 had more sales than 2022

**Monthly Average Price Over Time**

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/b5ca9768-6731-4658-87ff-c1b38b38e8bf)

### Explore Realtionships Between Variables 
**Correlation Between Price and Annual Income**

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/dd2268f9-88d2-49b9-b35e-ff5af88fe82f)

**Grouped Analysis By Gender - Average Price and Sales Count

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/eee4e20d-b560-47d7-abde-fe991b3000e9)

**Regional Sales Analysis - Average Price and Sales Count**

![image](https://github.com/wadegroux/Car-Sales-Portfolio-Project/assets/157087862/6cf15977-203e-4be6-a6dc-0538aa3100c5)

## Data Modeling 

