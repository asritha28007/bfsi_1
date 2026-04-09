# Banking Transactions Analysis (MySQL)

##  Overview

This project is a simple **banking database system** built using MySQL.
It stores customer details and their transactions, and performs various SQL queries for analysis.

---

## Database Structure

### 1. **Customer Table**

Stores customer details:

* `customer_id` (Primary Key)
* `name`
* `email` (Unique)
* `city`
* `account_type` (Savings / Current)
* `account_balance`

---

### 2. **Transactions Table**

Stores transaction details:

* `transaction_id` (Primary Key)
* `customer_id` (Foreign Key)
* `amount`
* `transaction_type` (credit/debit)
* `transaction_mode` (UPI, ATM, etc.)
* `transaction_date`

---

##  Queries Implemented

###  Basic Queries

* Fetch customers with balance > 1500
* Display all transactions sorted by date (latest first)
* Get unique transaction modes

---

###  Intermediate Queries

* Fetch top 5 highest transactions
* Find customers whose name starts with 'A'
* Calculate total transaction amount per customer

---

### Advanced Queries

* Find customers with total transaction > 100
* Join customer & transaction data
* Running total of transactions using window functions
* Rank customers based on account balance using `DENSE_RANK()`
* Find customers whose average transaction is above overall average

---

##  Concepts Used

* DDL (CREATE DATABASE, CREATE TABLE)
* DML (INSERT)
* Constraints (PRIMARY KEY, FOREIGN KEY, UNIQUE)
* Aggregate Functions (`SUM`, `AVG`)
* Joins
* Window Functions (`DENSE_RANK`, `SUM OVER`)
* Subqueries

---

##  How to Run

1. Create database:

```sql
CREATE DATABASE bank_system;
USE bank_system;
```

2. Run table creation queries

3. Insert data into tables

4. Execute SELECT queries for analysis

---

##  Output

The queries generate insights such as:

* High-value customers
* Transaction trends
* Customer rankings
* Spending behavior

---

##  Conclusion

This project demonstrates how SQL can be used for:

* Data storage
* Data analysis
* Real-world banking insights

---

✨ Simple but powerful SQL project for beginners.
