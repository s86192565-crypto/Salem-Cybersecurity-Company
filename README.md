# Salem Cybersecurity Company – Relational Database (SQL)

A relational database designed for a fictional cybersecurity company, **Salem**. The project models the company's core data (for example employees, clients, services, and security incidents) in 9 linked tables, and demonstrates database design and SQL querying skills.

> **Project type:** Academic / personal project
> **Tool:** MySQL
> **Author:** Ali Algamdi – AI Diploma student, Al-Baha University

---

## 📌 Project Overview

The goal of this project is to design a clean, well-structured database that stores and manages the information of a cybersecurity company, and to practice writing queries that answer real business questions.

This project covers:

- Database design and table relationships
- Data integrity using constraints
- Populating tables with sample data
- Writing queries from basic to intermediate level

---

## 🗂️ Database Structure

The database contains **9 tables**, connected through **primary keys** and **foreign keys**.

| # | Table Name | Purpose |
|---|------------|---------|
| 1 | `[table_1]` | [what it stores] |
| 2 | `[table_2]` | [what it stores] |
| 3 | `[table_3]` | [what it stores] |
| 4 | `[table_4]` | [what it stores] |
| 5 | `[table_5]` | [what it stores] |
| 6 | `[table_6]` | [what it stores] |
| 7 | `[table_7]` | [what it stores] |
| 8 | `[table_8]` | [what it stores] |
| 9 | `[table_9]` | [what it stores] |

### Relationships

- `[table_A]` → `[table_B]` (one-to-many): [short explanation]
- `[table_C]` → `[table_D]` (one-to-many): [short explanation]
- `[table_E]` ↔ `[table_F]` (many-to-many via `[table_G]`): [short explanation]

---

## 🔒 Data Integrity & Constraints

To keep the data accurate and consistent, the following constraints were applied:

| Constraint | Usage |
|-----------|-------|
| **PRIMARY KEY** | Uniquely identifies each record in every table |
| **FOREIGN KEY** | Links related tables and keeps references valid |
| **NOT NULL** | Prevents missing values in required columns (e.g. `[column]`) |
| **CHECK** | Restricts values to valid ranges/conditions (e.g. `[column]`) |
| **ENUM** | Limits a column to a fixed set of values (e.g. `[column]`: `'[value1]'`, `'[value2]'`, `'[value3]'`) |

---

## 🧪 Sample Data

Every table was populated with realistic sample data using `INSERT` statements, so that all queries can be tested and return meaningful results.

---

## 🔍 SQL Queries

The project includes queries that demonstrate the following concepts:

| Concept | Description |
|---------|-------------|
| `SELECT` | Retrieve specific columns and records |
| `JOIN` | Combine data from multiple related tables |
| **Subqueries** | Use a query inside another query to filter or compare results |
| `COUNT` / `SUM` | Calculate totals and statistics |
| `ORDER BY` | Sort results in ascending or descending order |
| `LIKE` | Search for text patterns |
| `UPDATE` | Modify existing records |

### Example Queries

**1. Retrieve data using JOIN**
```sql
-- [Describe what this query does]
SELECT ...
FROM [table_A]
JOIN [table_B] ON [table_A].id = [table_B].[foreign_key];
```

**2. Count records using COUNT**
```sql
-- [Describe what this query does]
SELECT [column], COUNT(*) AS total
FROM [table]
GROUP BY [column];
```

**3. Subquery**
```sql
-- [Describe what this query does]
SELECT ...
FROM [table]
WHERE [column] > (SELECT AVG([column]) FROM [table]);
```

**4. Search using LIKE**
```sql
-- [Describe what this query does]
SELECT *
FROM [table]
WHERE [column] LIKE '%[text]%';
```

**5. Update a record**
```sql
-- [Describe what this query does]
UPDATE [table]
SET [column] = '[new_value]'
WHERE id = [value];
```

---

## 📁 Repository Files

```
├── README.md        → Project documentation
├── schema.sql       → Table creation (CREATE TABLE) with constraints
├── data.sql         → Sample data (INSERT statements)
└── queries.sql      → SELECT, JOIN, subqueries, COUNT/SUM, ORDER BY, LIKE, UPDATE
```

---

## ▶️ How to Run

1. Install **MySQL** (or use MySQL Workbench).
2. Create a new database:
   ```sql
   CREATE DATABASE salem_cybersecurity;
   USE salem_cybersecurity;
   ```
3. Run the files in this order:
   1. `schema.sql`
   2. `data.sql`
   3. `queries.sql`

---

## 🎯 What I Learned

- Designing a relational database from scratch and planning table relationships
- Using constraints to protect data quality
- Writing queries to extract useful information from multiple tables
- Organizing and documenting a project clearly

---

## 🚀 Possible Improvements

- Add an ER diagram (Entity-Relationship) to visualize the design
- Add `VIEW`s and `INDEX`es to improve readability and performance
- Add stored procedures for common operations
- Connect the database to a simple web interface

---

## 👤 Author

**Ali Algamdi**
AI Diploma Student – Al-Baha University
📧 s86192565@gmail.com
