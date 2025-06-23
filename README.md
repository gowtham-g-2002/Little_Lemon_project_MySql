# 🍋 Little Lemon - MySQL Database Project

Welcome to the **Little Lemon Restaurant** database project — a SQL-based solution simulating real-world operations of a Mediterranean restaurant based in Chicago, Illinois.

## 🧰 Technologies Used
- MySQL (Structured Query Language)

## 📖 Project Overview

This project models the core operations of **Little Lemon**, including customer management, booking systems, courses offered, delivery addresses, and analytics using SQL queries, views, subqueries, and stored procedures.

---

## 📂 Database Structure

### 1. `Customers`
Stores customer info including `CustomerID`, `FullName`, and `PhoneNumber`.

### 2. `Bookings`
Tracks table reservations with fields like `BookingID`, `BookingDate`, `TableNumber`, and `CustomerID`.

### 3. `Courses`
Menu items with `CourseName`, `Cost`, and later an added `Ingredients` column.

### 4. `DeliveryAddress`
Includes customer delivery details with a foreign key relationship to `Customers`.

---

## ⚙️ SQL Features Demonstrated

✅ Database Creation  
✅ Table Design & Data Insertion  
✅ Data Filtering using `WHERE`, `BETWEEN`  
✅ `JOIN` operations  
✅ `GROUP BY` Aggregations  
✅ `REPLACE INTO` for Updates  
✅ `ALTER TABLE` for Modifications  
✅ `FOREIGN KEY` Constraints  
✅ `SUBQUERY` for Nested Logic  
✅ `VIEWS` for Virtual Tables  
✅ `STORED PROCEDURES` for Reusability  
✅ `CONCAT()` for String Manipulations  

---

## 🔍 Sample Query Highlights

```sql
-- View all customers
SELECT * FROM Customers;

-- Get all bookings between specific dates
SELECT * FROM Bookings 
WHERE BookingDate BETWEEN '2021-11-11' AND '2021-11-13';

-- Join Customers with Bookings
SELECT Customers.FullName, Bookings.BookingID 
FROM Customers RIGHT JOIN Bookings 
ON Customers.CustomerID = Bookings.CustomerID 
WHERE BookingDate = '2021-11-11';
📊 Use Cases
Restaurant management system mock-up

SQL training & interview practice

Data analysis foundation for Power BI dashboards

📎 How to Use
Import the provided SQL script into your MySQL environment.

Run the statements sequentially.

Experiment with custom queries or integrate into an app.

👨‍💻 Author
Gowtham G
GitHub: gowtham-g-2002
LinkedIn: https://www.linkedin.com/in/gowtham-gnanasekar/
📁 File
Little_Lemon_Project_mysql.sql – Full SQL script for this project
