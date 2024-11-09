# CIS_4400_HW
Campaign Finance:

## Business requirement:
Business Requirements: What is the distribution of the money campaign across donors/their employers.

## Functional requirement:
1.	Identify the number of donors and employers
2.	Categorize donors belonging to their employers
3.	Calculate the amount of money across donors, employers contributed.
4.	Compare the concentration of donors/employers’ contribution to the money campaign. 

## Data requirement:
The dataset should include transactions of each transactor and information about their employers.

## Information Architecture:

**Information Architecture Diagram** 
<img width="894" alt="Screen Shot 2024-11-08 at 8 44 12 PM" src="https://github.com/user-attachments/assets/357ad88f-6dfc-4cce-9bcc-50e8d14da9ae">



**Information Architecture Description** 

I will be doing a descriptive analytic by using OLAP. Stakeholder, personnel or even public should have the permission to access the data to know the prospect for the future campaign by knowing the distribution across donors and employers. However, only the city clerks can have the permission to update the data.

My first stage is to gather data from city of Austin, then clean, reformat, transform, and load them to data warehouse. The second stage will be data franchising, which I will filter data, restructure, metric calculation, summarize and store them into data warehouse. When I finished this process, the data is ready to be use for OLAP to do business analysis/reports/data visualization etc.


## Data Architecture:

**Data Architecture Diagram** 
<img width="808" alt="Screen Shot 2024-11-08 at 9 46 01 PM" src="https://github.com/user-attachments/assets/5b7331c4-499c-47a4-a198-7e42927fe34f">

**Data Architecture Description** 

The original data is collected by the city clerk and provided by the city of Austin. The dataset I received is already integrated, which includes the transaction type, name, amount, location, date, etc. However, data, can’t directly be used, so it still need ETL, filter and reformate the data that it’s needed. I will using the Top-Bottom approach to store data in data warehouse.  Then separate into two data marts, which transaction type of “contribution” will be in one data mart, and other transaction types will be in another mart since we will be focusing on the transaction type of contribution to do BI analysis for now.



## Dimensional Modeling:






