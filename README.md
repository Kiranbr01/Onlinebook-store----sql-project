# 📚 Online Bookstore SQL Project

## 📖 Overview
This project focuses on building and analyzing an **Online Bookstore Database** using **MySQL**.  
It demonstrates how to design a normalized relational database, import real-world data from CSV files, and perform **SQL operations** to gain insights about book sales, customer behavior, and revenue performance.

The project covers the full process — from **database creation and data import** to **advanced analytical queries** using various SQL techniques.

---

## 🧱 Database Design

The database is built around three relational tables — `Books`, `Customers`, and `Orders` — connected through **primary and foreign keys**.

### 🗂️ Tables Overview

#### 1. `Books`
| Column | Type | Description |
|--------|------|-------------|
| Book_ID | SERIAL PRIMARY KEY | Unique identifier for each book |
| Title | VARCHAR(100) | Book title |
| Author | VARCHAR(100) | Author name |
| Genre | VARCHAR(50) | Book category or genre |
| Published_Year | INT | Year of publication |
| Price | NUMERIC(10,2) | Price per book |
| Stock | INT | Quantity available in stock |

#### 2. `Customers`
| Column | Type | Description |
|--------|------|-------------|
| Customer_ID | SERIAL PRIMARY KEY | Unique identifier for each customer |
| Name | VARCHAR(100) | Customer name |
| Email | VARCHAR(100) | Customer email |
| Phone | VARCHAR(15) | Contact number |
| City | VARCHAR(50) | Customer’s city |
| Country | VARCHAR(150) | Customer’s country |

#### 3. `Orders`
| Column | Type | Description |
|--------|------|-------------|
| Order_ID | SERIAL PRIMARY KEY | Unique identifier for each order |
| Customer_ID | INT | References `Customers(Customer_ID)` |
| Book_ID | INT | References `Books(Book_ID)` |
| Order_Date | DATE | Date of order |
| Quantity | INT | Number of books purchased |
| Total_Amount | NUMERIC(10,2) | Total value of order |

---

## ⚙️ What We Did in This Project

- **Created the database** `OnlineBookstore` using MySQL Workbench.  
- **Designed and implemented relational tables** with proper constraints.  
- **Imported datasets** from CSV files into each table.  
- **Validated data** and ensured referential integrity with primary and foreign keys.  
- **Executed SQL queries** to analyze customer and sales data.  
- **Derived business insights** such as sales trends, customer behavior, and stock movement.

---

## 🧩 SQL Operations and Techniques Used

This project uses a wide range of SQL operations to analyze data effectively:

| Operation | Description |
|------------|-------------|
| **SELECT & WHERE** | To fetch and filter data based on conditions |
| **JOIN (INNER, LEFT, RIGHT)** | To combine data from multiple related tables |
| **GROUP BY & HAVING** | To group and aggregate data for reporting |
| **ORDER BY & LIMIT** | To sort and retrieve specific data subsets |
| **Aggregate Functions** | Used `SUM()`, `COUNT()`, `AVG()`, `MAX()`, and `MIN()` for calculations |
| **Subqueries** | Used for nested calculations and comparisons |
| **Window Functions** | Applied `RANK()` and cumulative calculations for ranking and trends |
| **Data Filtering** | Used operators like `BETWEEN`, `IN`, and pattern matching with `LIKE` |
| **Mathematical & Logical Expressions** | Used to calculate total amounts, averages, and percentages |

---

## 💡 Key Insights Derived

- Total **revenue** generated from all orders.  
- **Most popular genres** and top-selling books.  
- **Top customers** based on total spending.  
- **Author performance** based on sales quantity and revenue.  
- **Stock utilization** and books with lowest remaining inventory.  
- **Customer distribution** across countries and cities.  
- **Average order value** and customer purchase frequency.  
- **Top 3 most expensive books** within each genre.  

---

## 🧰 Tools and Technologies
- **Database:** MySQL  
- **Environment:** MySQL Workbench  
- **Data Source:** Books.csv, Customers.csv, Orders.csv  
- **Concepts Used:** Joins, Aggregations, Subqueries, Window Functions, Ranking, Filtering  


 



