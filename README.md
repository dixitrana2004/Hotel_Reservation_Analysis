# Hotel Reservation Analysis with SQL

A SQL-based data analysis project exploring guest preferences, booking trends, and operational insights from a hotel reservation dataset.

## 📌 Overview

The hotel industry relies on data to make informed decisions and improve guest experience. This project uses SQL to query and analyze a hotel reservation dataset in order to answer 15 business-relevant questions about bookings, pricing, guest demographics, and seasonal trends.

## 📂 Repository Contents

| File | Description |
|---|---|
| `Hotel_Reservation_Dataset.csv` | Raw dataset containing ~700 hotel reservation records |
| `Hotel_Reservation_Query.sql` | SQL script with table setup and all 15 analysis queries |
| `Problem_Statement_-_Hotel_Reservation_Analysis.pdf` | Original project brief and list of questions |
| `README.md` | Project documentation (this file) |

## 🗃️ Dataset Details

The dataset includes the following columns:

| Column | Description |
|---|---|
| `Booking_ID` | Unique identifier for each reservation |
| `no_of_adults` | Number of adults in the reservation |
| `no_of_children` | Number of children in the reservation |
| `no_of_weekend_nights` | Number of weekend nights booked |
| `no_of_week_nights` | Number of weekday nights booked |
| `type_of_meal_plan` | Meal plan selected by guests |
| `room_type_reserved` | Type of room reserved |
| `lead_time` | Days between booking date and arrival date |
| `arrival_date` | Date of arrival |
| `market_segment_type` | Market segment of the booking (Online, Offline, Corporate, etc.) |
| `avg_price_per_room` | Average price per room (in dataset currency) |
| `booking_status` | Final status of the booking (Confirmed / Not_Canceled / Canceled) |

## 🛠️ Tools Used

- **MySQL** for querying and analysis
- **SQL** features used: `GROUP BY`, `ORDER BY`, aggregate functions (`COUNT`, `AVG`, `SUM`, `MAX`, `MIN`), subqueries, `HAVING`, and date functions (`YEAR()`, `MONTH()`, `MONTHNAME()`)

## ❓ Business Questions Answered

1. Total number of reservations in the dataset
2. Most popular meal plan among guests
3. Average price per room for reservations involving children
4. Number of reservations made for a given year
5. Most commonly booked room type
6. Number of reservations that include weekend nights
7. Highest and lowest lead time for reservations
8. Most common market segment type
9. Number of reservations with booking status "Confirmed"
10. Total number of adults and children across all reservations
11. Average number of weekend nights for reservations involving children
12. Number of reservations made in each month of the year
13. Average number of weekend/weekday nights spent, by room type
14. Most common room type for reservations involving children, and its average price
15. Market segment type generating the highest average price per room

## 🚀 How to Run

1. Create a database (e.g. `sql_hotel`) in MySQL:
   ```sql
   CREATE DATABASE sql_hotel;
   USE sql_hotel;
   ```
2. Import `Hotel_Reservation_Dataset.csv` into a table named `hotel reservation dataset` (use MySQL Workbench's **Table Data Import Wizard** or `LOAD DATA INFILE`).
3. Open `Hotel_Reservation_Query.sql` in your SQL client.
4. Run the queries sequentially — each question is labeled with a comment (`# 1.`, `# 2.`, etc.) above its corresponding query.
   
## 📊 Key Insights (Sample)

- Identified the most popular meal plan and room type among guests.
- Found how lead time (days between booking and arrival) varies, highlighting last-minute vs. early bookers.
- Determined which market segment (Online, Offline, Corporate, etc.) drives the highest room prices.
- Quantified seasonal booking trends by month and year.
- Compared booking patterns for families (with children) vs. other guests.

## 🎯 Project Purpose

This project was completed as part of a data analysis internship/practice exercise to strengthen SQL querying skills — including aggregation, grouping, subqueries, and date manipulation — using a real-world style hotel booking dataset.

