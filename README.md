# Omnify-Sample-Data-Dashboard

![image](https://github.com/user-attachments/assets/7820a654-8a74-4caa-a177-a600b3a7c5a9)

## Overview
This project involves analyzing a raw dataset containing booking information for a multi-service business, including class bookings, subscriptions, facility rentals, and birthday party reservations. The dataset was cleaned and processed using PostgreSQL and Excel, addressing inconsistencies and missing values. Key insights were derived through exploratory data analysis (EDA), and an interactive dashboard was built in Power BI to visualize revenue trends, customer preferences, and booking patterns. The repository includes SQL queries, data cleaning steps, the Power BI dashboard file, and a detailed report documenting the entire workflow.

## Problem Statement
A multi-service business requires a data-driven approach to optimize its booking management and revenue tracking. The existing raw dataset, containing class bookings, subscriptions, facility rentals, and birthday party reservations, is inconsistent, incomplete, and unstructured. Without proper data cleaning and analysis, identifying key trends, customer preferences, and revenue-generating services becomes challenging. This project aims to clean, analyze, and visualize the dataset through an interactive Power BI dashboard, enabling stakeholders to make informed decisions based on booking trends, customer behavior, and revenue insights.

## Dataset
The dataset consists of booking information , covering various services such as class bookings, subscriptions, facility rentals, and birthday party reservations. The dataset is structured with multiple columns, each representing different attributes related to bookings, customers, and services. Given its real-world nature, the dataset contains inconsistencies, missing values, and redundant information that require cleaning and preprocessing.

![image](https://github.com/user-attachments/assets/dad80c12-ff1b-4d03-9d78-dd0432df8589)

## Loading the Dataset
• PostgressSQL and Excel were used for EDA of the dataset.<br>
•	Converted .xlsx file to .csv using excel.<br>
•	Created a new schema named internship_assignment in Postgress.<br>
•	Select table and open Query Tab.<br>
•	In Query write the query to create table with necessary columns and data types.<br>
•	When table is created load dataset namely the .csv file created.<br>

![image](https://github.com/user-attachments/assets/485a2ab1-13aa-4b92-9a58-b7c5fe091c76)

## Exploratory Data Analysis
• The dataset was explored using PostgreSQL and Excel to identify inconsistencies, missing values, and patterns.<br>
• The subscriptiontype column contained all null values and was dropped.<br>
• The price column was sorted to check for anomalies, and entries with a price of 0 were removed.<br>
• The status column had 462 entries marked as Pending and 423 as Confirmed.<br>
• Columns theme, instructor, and classtype contained partial null values; separate datasets were created for non-null values.<br>
• The dataset was exported as .csv files after cleaning for dashboard creation in Power BI.<br>








