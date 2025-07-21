# Zentrix Technologies Sales Insights PowerBi Dashboard

## Problem Statement:
Zentrix Technologies  is a Hardware company which delivers computer hardware & peripheral Manufacturers to his clients, which has several branches throughout India. The sales director of the company is facing a lot of issues in terms of understanding how the business is performing and what are all the problem company is facing currently as the sales are not as expected and declining gradually. And whenever he calls the regional managers to get the current status of the sales and market, as a human behaviour, these people sugar cote the truth and send tons of Excel files instead of disclosing the truth, which made the sales director more frustrated. Humans are not comfortable in consuming numbers from excel files, which is obvious reason for the frustration.

## Solution:
Sales director of the Zentrix Technologies, decided to build a PowerBI Dashboard for converting the data into visual representation to make data driven decisions.

## AIMS Grid:
By using the AIMS grid project management tool, we made sure what are the purpose, stakeholder, end result and success criteria of our project.

<img width="1024" height="1024" alt="AIMS-Grid" src="https://github.com/user-attachments/assets/3f91aaf7-717b-4ead-a9aa-959fe1014a39" />


## Steps Followed in this project:
1. Performed a High level analysis of data in SQL to get better understanding over the data.
2. Connected the SQL data set to PowerBI.
3. Performed ETL and data cleaning on the imported data.
4. In the currency there were two types of currencies in transactions, performed currency conversion to make all the currency type same
5. Created measure for needs and used them for creating visuals in PowerBi.
6. After the initial report reviewed by the stakeholders, made changes to the report based on the review commends.

## Measures Created for Succesfull Completion of Analysis:
1. Profit Contribution % = DIVIDE([Total Profit Margin],CALCULATE([Total Profit Margin],all('sales customers'),all('sales markets'),all('sales products')))
2. Profit Margin % = DIVIDE([Total Profit Margin],[Total Revenue],0)
3. Revenue Contribution % = DIVIDE([Total Revenue],CALCULATE([Total Revenue],all('sales customers'),all('sales markets'),all('sales products')))
4. Total Profit Margin = sum('sales transactions'[profit_margin])
5. Total Quantity = sum('sales transactions'[sales_qty])
6. Total Revenue = sum('sales transactions'[Normalized_Currency])

# Final Result:
## Revenue Insights Page:

<img width="1956" height="1074" alt="Revenue Insights Page" src="https://github.com/user-attachments/assets/4716f139-27c2-45ff-a36f-c747221f277b" />

## Profit Insights Page:

<img width="2214" height="1230" alt="Profit Insights Page" src="https://github.com/user-attachments/assets/f98cb95a-706e-48ed-aaa9-8cef1f72cf93" />

## Perfomance Insights Page:

<img width="2223" height="1233" alt="Perfomance Insights Page" src="https://github.com/user-attachments/assets/6dc578ad-f8af-41f7-8b3a-4266136b66fe" />

## Prediction Insights Page:

<img width="2224" height="1227" alt="Prediction Insights" src="https://github.com/user-attachments/assets/8dae41c4-644d-40ca-9ae5-86e659f5a701" />


# Final Report:
![Report-GIF](https://github.com/user-attachments/assets/21a40fb5-ee7c-497b-b345-28e5172d03ff)


## Insights from this Project:

- Revenue consistently declined in the year 2020.
- The Delhi market contributes the highest revenue share at 52.8%, while the Surat market delivers a stronger profit margin of 4.86%. Therefore, we may consider focusing more on Surat for profitability.
- Although Delhi’s profit margin is lower at 2.30% compared to Surat, it still contributes the highest share of overall profit at 48%.
- The Central Zone offers a higher profit margin percentage than both the North and South Zones.
- Brick & Mortar customers generate more revenue than those from the E-Commerce segment.
- Our top-performing customer is ElectricalSara Stores, contributing 42% of overall revenue, with a profit margin of 2.25% and accounting for 38% of Zentrix’s total profit contribution.
- January shows the highest revenue across all years, while September records the lowest.
