
# Project Title

## Energy Consumption Dashboard

##Snapshot for Energy Consumption Dashboard
![Energy_consumption_ss](https://github.com/Siddhi-Zore12/Data-Analysis_dashboard/assets/128132433/737c6052-bff6-4641-8c5f-deb7e7cf4baa)


## Problem Statement

The dashboard is created to analyze data of energy consumption of electricity,gas,water of some cities in USA. This dashboard helps the organization to know in which area energy consumption is more. Through dashboard, one can recommend on how to optimize their energy usage. This could include identifying areas for efficiency improvements, such as upgrading equipment, implementing energy-saving technologies, or adjusting usage patterns. It will also help to identify peak demand periods and work with clients to develop demand response strategies. This could involve encourage customers to reduce energy usage during peak times or coordinating with the grid to provide load-shifting services.

## Step followed
1. Dealing with null values and outlier either by removing (If only it will not give big impact while analyzing) or fill it with analyzing remaining data.

2. Load data into Power BI desktop.

3. Calculated Total Cost and Unit Consumed.
   
4.Since the data has 3 type consumption type namely electricity, gas and water using 100% Stacked Column Chart.

![Stacked_col_chart](https://github.com/Siddhi-Zore12/Data-Analysis_dashboard/assets/128132433/0eb06619-2ebe-45ea-86d4-29193ea41e67)


5. For Unit Consumption by Consumption Type, using donut-chart.
   
![Donut_chart](https://github.com/Siddhi-Zore12/Data-Analysis_dashboard/assets/128132433/5756105e-cb43-4b75-a452-82453b0e15e9)

6. For Unit Consumed by building, using Infographic designer.

![infographic](https://github.com/Siddhi-Zore12/Data-Analysis_dashboard/assets/128132433/7acecdbf-a9fc-4615-85e0-04c3eec05fd7)

7. From dynamic dashboard, we can state that 

 i. Los Angeles had 37,64,352.46 Total Cost. Unit Consumed by Electricity is approx 5 Millions, Water is approx 45 Millions(88.62%) and remaining by gas is 604k.

 ii. Pheonix had 13,32,878.14 Total Cost. Unit Consumed by Electricity is approx 2 Millions, Water is approx 16 Millions(88.62%) and remaining by gas is 194k.

 iii. Houston had 12,76,742.58 Total Cost. Unit Consumed by Electricity is approx 2 Millions, Water is approx 16 Millions(88.62%) and remaining by gas is approx 200k.

 iv. Chicago had 38,19,369.46 Total Cost. Unit Consumed by Electricity is approx 5 Millions(10.19%), Water is approx 45 Millions(88.62%) and remaining by gas is 627k.

 v. New York had 38,43,352.70 Total Cost. Unit Consumed by Electricity is approx 5 Millions(10.19%), Water is approx 46 Millions(88.62%) and remaining by gas is 628k.

8. For Calculating Total Cost and Unit Consumed used DAX function in Measures
 i. Total Cost = SUMX('Energy Consumptions', 'Energy Consumptions'[Unit]* RELATED(Rates[Price Per Unit]))
 ii. Unit consumed = SUM('Energy Consumptions'[Unit])


