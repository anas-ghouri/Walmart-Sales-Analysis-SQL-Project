# Walmart-Sales-Data-Analysis-SQL-Project

## Project Scope:
Perform in-depth sales analysis to uncover business insights that highlight performance trends and identify growth opportunities and recommend data-driven strategies for improving product sales. The main goal of this project is to gain insights sales data, exploring the various factors that influence sales across different branches.

## About Data
This project's data was obtained from the Kaggle Walmart Sales Forecasting Competition and it encompasses sales transactions from three Walmart branches situated in Mandalay, Yangon, and Naypyitaw, respectively.

The data contains 17 columns and 1000 rows:
| Column            | Description                                   | Data Type        |
|-------------------|-----------------------------------------------|------------------|
| invoice_id        | Invoice of the sales made                     | VARCHAR(30)      |
| branch            | Branch at which sales were made               | VARCHAR(5)       |
| city              | The location of the branch                    | VARCHAR(30)      |
| customer_type     | The type of the customer                       | VARCHAR(30)      |
| gender            | Gender of the customer making purchase        | VARCHAR(10)      |
| product_line      | Product line of the product sold               | VARCHAR(100)     |
| unit_price        | The price of each product                     | DECIMAL(10, 2)   |
| quantity          | The amount of the product sold                 | INT              |
| VAT               | The amount of tax on the purchase             | FLOAT(6, 4)      |
| total             | The total cost of the purchase                | DECIMAL(12, 4)   |
| date              | The date on which the purchase was made       | DATETIME         |
| time              | The time at which the purchase was made       | TIME             |
| payment           | The total amount paid                         | DECIMAL(10, 2)   |
| cogs              | Cost Of Goods sold                            | DECIMAL(10, 2)   |
| gross_margin_pct  | Gross margin percentage                       | FLOAT(11, 9)     |
| gross_income      | Gross Income                                  | DECIMAL(12, 4)   |
| rating            | Rating                                        | FLOAT(2, 1)      |


## Analysis Flow:

# 1. Product Analysis
Analyzed product line performance to identify top contributors to revenue and profit, while highlighting areas for strategic improvement.

# 2. Sales Analysis
Evaluated sales trends across time, branches, and payment channels to assess the effectiveness of sales strategies and uncover opportunities for revenue growth.

# 3. Customer Analysis
Segmented customers to understand buying behavior, analyze revenue contribution by segment, and uncover actionable insights to optimize customer engagement and profitability.


## Approach Used

***1.	Data Wrangling***

During this initial phase, the data is examined to detect any NULL or missing values, and strategies for data replacement are implemented to address and substitute these values effectively.

- Build a database
- Create a table and insert the data.
- Select columns with null values in them. Null values are not present in our database because, in creating the tables, NOT NULL was specified for each field, effectively filtering out any null values.

***2.	Feature Engineering***

Derived new columns from existing data for time-based analysis:

time_of_day: Categorized transactions into Morning, Afternoon, and Evening to analyze peak sales periods during the day.

day_name: Extracted weekday names to identify branch activity trends across the week.

month_name: Extracted month names to evaluate monthly sales and profitability performance.

***3.  Exploratory Data Analysis (EDA)***


## Business Questions to Answer

### Generic Questions
1.	How many distinct cities are present in the dataset?
2.	In which city is each branch situated?

### Product Analysis
1.	How many distinct product lines are there in the dataset?
2.	What is the most common payment method?
3.	What is the most selling product line?
4.	What is the total revenue by month?
5.	Which month recorded the highest Cost of Goods Sold (COGS)?
6.	Which product line generated the highest revenue?
7.	Which city has the highest revenue?
8.	Which product line incurred the highest VAT?
9.	Retrieve each product line and add a column product_category, indicating 'Good' or 'Bad,' based on whether its sales are above the average.
10.	Which branch sold more products than average product sold?
11.	What is the most common product line by gender?
12.	What is the average rating of each product line?

### Sales Analysis
1.	Number of sales made in each time of the day per weekday
2.	Identify the customer type that generates the highest revenue.
3.	Which city has the largest tax percent/ VAT (Value Added Tax)?
4.	Which customer type pays the most VAT?

### Customer Analysis
1.	How many unique customer types does the data have?
2.	How many unique payment methods does the data have?
3.	Which is the most common customer type?
4.	Which customer type buys the most?
5.	What is the gender of most of the customers?
6.	What is the gender distribution per branch?
7.	Which time of the day do customers give most ratings?
8.	Which time of the day do customers give most ratings per branch?
9.	Which day of the week has the best avg ratings?
10.	Which day of the week has the best average ratings per branch?

### Advanced Analytics
1. Is there a correlation between high ratings and higher gross income?
2. Which product line is most sensitive to time_of_day (i.e. shows the most variation in sales across different times)?
3. Which branch has the fastest-moving inventory (highest quantity sold relative to number of invoices)?
4. Month-over-Month Revenue Growth
5. Which product line shows the most variation in sales across different times of the day?
6. Which product line has the highest profit margin % 

    

