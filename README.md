# Credit-Card-Dashbaord
# 💳 Credit Card Financial Dashboard 📊

## Project Overview

This project focuses on developing an interactive credit card financial dashboard using **Power BI**, integrated with a **SQL database**. The primary goal is to transform raw transaction and customer data into actionable insights, enabling stakeholders to monitor key performance metrics and trends in real-time to support informed decision-making.

This repository showcases the end-to-end data process, from data acquisition and SQL querying to dashboard development and insights generation.

## Key Features & Learnings

* **Interactive Dashboard Development:** Created dynamic and user-friendly dashboards in Power BI for comprehensive financial analysis.
* **SQL Database Integration:** Seamlessly connected Power BI to a SQL database to pull and process real-time transaction and customer data.
* **Real-time Insights Generation:** Designed the dashboard to provide up-to-date views on credit card financial performance.
* **Data Processing & Analysis:** Streamlined data processing pipelines and performed in-depth analysis to identify key performance metrics (KPIs) and emerging trends.
* **Stakeholder Communication:** Developed skills in sharing clear, concise, and actionable insights derived from dashboard findings to support business decision-making processes.

## Technologies Used

* **Business Intelligence:** Power BI
* **Database Management:** SQL (specific dialect like Oracle, MySQL, PostgreSQL based on demonstrated queries)
* **Data Extraction & Transformation:** SQL queries, Data modeling within Power BI
* **Version Control:** Git & GitHub

## Data Overview

The project utilizes comprehensive transaction and customer datasets. An example of the raw data structure is shown below:

![Sample Data Overview](https://github.com/decoder2201/Credit-Card-Dashbaord/blob/main/Screenshot%202025-06-01%20212703.png)
(https://github.com/decoder2201/Credit-Card-Dashbaord/blob/main/Screenshot%202025-06-01%20212641.png)


## SQL Query Examples

Data was efficiently extracted and transformed using SQL queries. Here are examples of the SQL logic employed for data manipulation and analysis:

### Creation & Insertion Data

```sql
CREATE DATABASE ccdb;
Create cc_detail table;
Create cust_detail table;

-- 2. Create cc_detail table

CREATE TABLE cc_detail (
    Client_Num INT,
    Card_Category VARCHAR(20),
    Annual_Fees INT,
    Activation_30_Days INT,
    Customer_Acq_Cost INT,
    Week_Start_Date DATE,
    Week_Num VARCHAR(20),
    Qtr VARCHAR(10),
    current_year INT,
    Credit_Limit DECIMAL(10,2),
    Total_Revolving_Bal INT,
    Total_Trans_Amt INT,
    Total_Trans_Ct INT,
    Avg_Utilization_Ratio DECIMAL(10,3),
    Use_Chip VARCHAR(10),
    Exp_Type VARCHAR(50),
    Interest_Earned DECIMAL(10,3),
    Delinquent_Acc VARCHAR(5)
);


-- 2. Create cust_detail table

CREATE TABLE cust_detail (
    Client_Num INT,
    Customer_Age INT,
    Gender VARCHAR(5),
    Dependent_Count INT,
    Education_Level VARCHAR(50),
    Marital_Status VARCHAR(20),
    State_cd VARCHAR(50),
    Zipcode VARCHAR(20),
    Car_Owner VARCHAR(5),
    House_Owner VARCHAR(5),
    Personal_Loan VARCHAR(5),
    Contact VARCHAR(50),
    Customer_Job VARCHAR(50),
    Income INT,
    Cust_Satisfaction_Score INT
);


