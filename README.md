# **Bank Customer Churn Analysis**
![image](https://github.com/GarimaGupta0614/BankCustomerChurnAnalysis_PowerBI/assets/58433278/33b47f5b-ac6f-4d65-baf7-d1769fe29184)
![image](https://github.com/GarimaGupta0614/BankCustomerChurnAnalysis_PowerBI/assets/58433278/3171ad1b-0987-411b-ac57-d5aaeebfc08c)
![image](https://github.com/GarimaGupta0614/BankCustomerChurnAnalysis_PowerBI/assets/58433278/282e523d-6b6c-4116-807e-d64cdc4eeeec)
![image](https://github.com/GarimaGupta0614/BankCustomerChurnAnalysis_PowerBI/assets/58433278/b06a1a4f-5b6f-441a-9380-4d011384e361)

## Business task:
Analyse the data and bring out insights to know what leads a client towards the decision to leave the Bank as churn prevention allows companies to develop loyalty programs and retention campaigns to keep as many customers as possible.

## Information about data set:
Data is available as 5 excel files and 2 .csv files for the years 2018-2021.

1. ActiveCustomer.xlsx - Dimension table with two columns: ActiveID and ActiveCategory.
2. CreditCard.xlsx - Dimension table with two columns: CreditID and Category.
3. Gender.xlsx - Dimension table with two columns: GenderID and Gendercategory.
4. ExitCustomer.xlsx - Dimension table with two columns: ExitID and ExitCategory.
5. Geography.xlsx - Dimension table with two columns: GeographyID and GeographyLoaction.
6. CustomeInfo.csv - Dimension table with two columns: CustomerID and Surname.
7. Bank_Churn.csv - Fact table with 14 columns and 10,000 rows.

## Data processing and cleaning:
1. Loaded all the files in PowerBI desktop.
2. Checked all the column types.
3. Checked Bank_Churn and CustomerInfo tables for duplicate rows and null values.
4. Removed RowNumber column from Bank_Churn table as it is not required for analysis.
5. Created new column CreditCategory in Bank_Churn table based on Bank_Churn.CreditScore using DAX.
6. Created a new DateMaster table with data from Bank_Churn.Bank_DOJ column. Columns in DateMaster table are: Date, year, month, monthname using DAX.
7. Created a new table Calculations with data from various tables. Measures in the Calculation table are: TotalCustomers, ExitCustomers, RetainCustomers, ActiveCustomers, InactiveCustomers, CreditCardHolders and NonCreditCardHolders using DAX.
Data modelling:
Established star schema relationship between fact table and dimension tables in Power Pivot.

## Findings:
1. Total number of customers associated with the bank are increasing by year.
2. Credit card holders are more likely to leave the bank.
3. Spain has seen the least number of exit customers in all the years.
4. No trend can be identified in terms of tenure of the customers.
5. Female customers are more likely to leave the bank.
6. Customers with balance more than 150K are less likely to leave the bank.
7. 64% of the customers who left the bank were inactive category.
8. Customers with less credit scores are more likely to leave the bank.
9. Most of the customers who left the bank fall in the age group 36 – 55 years as they also constitute the highest number of customers associated with the bank. 
10. Less the number of products a customer has purchased, more are his/her chances of leaving the bank.
11. Customers with estimated salary more than 1L are least likely to leave the bank.




