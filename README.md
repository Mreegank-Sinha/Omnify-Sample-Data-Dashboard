# Omnify-Sample-Data-Dashboard

![image](https://github.com/user-attachments/assets/7820a654-8a74-4caa-a177-a600b3a7c5a9)

## Overview
This project involves analyzing a raw dataset containing booking information for a multi-service business, including class bookings, subscriptions, facility rentals, and birthday party reservations. The dataset was cleaned and processed using PostgreSQL and Excel, addressing inconsistencies and missing values. Key insights were derived through exploratory data analysis (EDA), and an interactive dashboard was built in Power BI to visualize revenue trends, customer preferences, and booking patterns. The repository includes SQL queries, data cleaning steps, the Power BI dashboard file, and a detailed report documenting the entire workflow.

## Problem Statement
A multi-service business requires a data-driven approach to optimize its booking management and revenue tracking. The existing raw dataset, containing class bookings, subscriptions, facility rentals, and birthday party reservations, is inconsistent, incomplete, and unstructured. Without proper data cleaning and analysis, identifying key trends, customer preferences, and revenue-generating services becomes challenging. This project aims to clean, analyze, and visualize the dataset through an interactive Power BI dashboard, enabling stakeholders to make informed decisions based on booking trends, customer behavior, and revenue insights.

## Dataset
The dataset consists of booking information , covering various services such as class bookings, subscriptions, facility rentals, and birthday party reservations. The dataset is structured with multiple columns, each representing different attributes related to bookings, customers, and services. Given its real-world nature, the dataset contains inconsistencies, missing values, and redundant information that require cleaning and preprocessing.
<br>

![image](https://github.com/user-attachments/assets/dad80c12-ff1b-4d03-9d78-dd0432df8589)


## Loading the Dataset
• PostgressSQL and Excel were used for EDA of the dataset.<br>
•	Converted .xlsx file to .csv using excel.<br>
•	Created a new schema named internship_assignment in Postgress.<br>
•	Select table and open Query Tab.<br>
•	In Query write the query to create table with necessary columns and data types.<br>
•	When table is created load dataset namely the .csv file created.<br>
<br>

![image](https://github.com/user-attachments/assets/485a2ab1-13aa-4b92-9a58-b7c5fe091c76)


## Exploratory Data Analysis
• The dataset was explored using PostgreSQL and Excel to identify inconsistencies, missing values, and patterns.<br>
• The subscriptiontype column contained all null values and was dropped.<br>
<br>

![image](https://github.com/user-attachments/assets/91f05dee-4175-4936-bbe1-d128307111b9)

<br>
• The price column was sorted to check for anomalies, and entries with a price of 0 were removed.<br>
<br>

![image](https://github.com/user-attachments/assets/6abb1152-d205-4a7c-8c69-f535a8ac7409)

<br>
• The status column had 462 entries marked as Pending and 423 as Confirmed.<br>
<br>

![image](https://github.com/user-attachments/assets/c0620fce-faf3-4f2e-97ef-f08b3fce4e68)

<br>
• Columns theme, instructor, and classtype contained partial null values; separate datasets were created for non-null values.<br>
• The dataset was exported as .csv files after cleaning for dashboard creation in Power BI.<br>

## ETL
#### The prerequiste to ETL was to create three new datasets for proper analysis.
- Themes
- Instructor
- Class

Power BI was used for data transformation and visualization.<br>
The cleaned dataset was imported, along with separate datasets for theme, instructor, and classtype.<br>
A star schema was created to define relationships between tables.<br>
<br>

![image](https://github.com/user-attachments/assets/8959f55e-d02b-44e5-bcc2-4b41809be8fe)

<br>
A new column months was derived from bookingdate to format dates as “DD MMM YY” (e.g., 01 JUN 25).<br>
<br>

![image](https://github.com/user-attachments/assets/7f208c76-6fbe-4676-85fb-b5089e7674b8)

<br>
A measure for Total Revenue was created for financial analysis.<br>
<br>

![image](https://github.com/user-attachments/assets/c6cfaf89-eb9d-42db-bad2-aba84527c83b)

<br>
Quarterly groupings appeared unexpectedly in Power BI and were removed for accurate reporting.<br>

## Dashboard Creation
• A Total Revenue card was created to display overall earnings.<br>


![image](https://github.com/user-attachments/assets/08484be7-ed79-427a-a24a-a0a70f520def)


• Date sliders were added to filter bookings by month and date.<br>

![image](https://github.com/user-attachments/assets/e2c3a831-be68-4b90-935d-50ab2bd2a644)


• A bar chart showing revenue by customers helped identify top spenders.<br>


![image](https://github.com/user-attachments/assets/5fc11bf2-1c88-4499-a2ee-bba88f1f28db)


• A bar chart of booking type by date revealed popular services over time.<br>


![image](https://github.com/user-attachments/assets/68e815a6-8d4c-4a36-a9ea-d0bea2cb1125)


• A revenue by booking type chart highlighted high and low-earning services.<br>


![image](https://github.com/user-attachments/assets/1dd5d2a7-17d9-4822-89b8-26d15ed11dbd)


• A line graph of booking revenue trends showcased daily and monthly sales patterns.<br>


![image](https://github.com/user-attachments/assets/0062c1b6-f7ae-4b38-b90e-233cf8dc4474)


• A chart displaying bookings by time slot identified peak booking hours.<br>


![image](https://github.com/user-attachments/assets/12d9611f-f95f-429f-8745-e2bde48e0973)


• A Top 5 Customers chart highlighted the highest-paying customers.<br>


![image](https://github.com/user-attachments/assets/338c98e0-51d1-4bad-96c2-546251064944)


• Donut charts for classtype, instructor, and theme helped analyze customer preferences.<br>


![image](https://github.com/user-attachments/assets/fbf89305-68c5-47b5-a52d-f968abfd92c4)  ![image](https://github.com/user-attachments/assets/803e43b7-3458-4e04-afaf-78d0e6fec83e)


• Toggle buttons for Confirmed, Pending, and All Bookings allowed easy filtering.<br>

![image](https://github.com/user-attachments/assets/ee1bf3d9-b652-41d3-9356-dc74612a0d87)


• The final dashboard provided actionable insights on revenue, bookings, and customer trends.<br>

## INSIGHTS
Total revenue generated is: 139.48 thousand.<br>
Total revenue generated by confirmed booking is:  66.85 thousand.<br>
Total revenue generated by pending bookings is: 72.63 thousand.<br>
Most popular Instructor is James Howard.<br>
Most Popular class type is a tie between Dance and Gymnastics.<br>
Most Popular theme is Superhero.<br>
Top Customer is Customer 79.<br>
Sales in April were highest with value 46.69 thousand.<br>

