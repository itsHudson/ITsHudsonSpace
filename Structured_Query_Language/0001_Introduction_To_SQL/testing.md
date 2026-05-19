# 1. Introduction to SQL

> Level: 🟢 Beginner  
> Estimated Learning Time: 45–90 Minutes  
> Prerequisites:
>
> - Basic computer knowledge
> - Basic understanding of applications/websites
> - No programming experience required

---

# 1.1 SQL Fundamentals

SQL Fundamentals is the foundation of database learning.

Before learning:

- joins
- subqueries
- indexing
- optimization
- transactions
- warehousing

you must first understand:

- what SQL is
- why SQL exists
- where SQL is used
- how SQL connects with real applications

---

## 1.1.1 Learning Objectives

After completing this section, you should understand:

- what SQL is
- what databases are
- how SQL works
- why companies use SQL
- how SQL is used in applications
- the difference between SQL and NoSQL
- how SQL is used in backend systems
- how SQL is used in analytics and machine learning

---

# 1.2 What is SQL?

---

## Definition

SQL stands for:

**Structured Query Language**

SQL is a language used to communicate with relational databases.

Using SQL, users can:

- retrieve data
- insert data
- update data
- delete data
- create tables
- manage users
- control transactions

---

## Why SQL Exists

Before databases became modernized, managing records was difficult.

Companies needed a standard way to:

- store information
- organize records
- search data quickly
- update records safely

SQL became the universal language for structured data management.

---

## Real-Life Analogy

Think of a database like a school office filing system.

### Real-Life Structure

In a school office:

- A cabinet stores all records
- A folder stores one category
- A paper sheet stores one student record
- Each field stores one piece of information

Example student information:

- Student ID
- Student Name
- Age
- Course

---

## Database Equivalent

| Real-Life Item | Database Equivalent |
|---|---|
| Cabinet | Database |
| Folder | Table |
| Paper Sheet | Row |
| Information Field | Column |

---

## Example Table

Student table:

| student_id | name | age | course |
|---|---|---|---|
| 1 | John | 20 | IT |
| 2 | Sarah | 21 | Business |

---

## Understanding the Table

### Columns

Columns represent categories of information.

Example columns:

- `student_id`
- `name`
- `age`
- `course`

---

### Rows

Rows represent individual records.

Example rows:

- John's student record
- Sarah's student record

---

## What SQL Can Do

| Task | Purpose | SQL Command |
|---|---|---|
| Retrieve Data | Read information | `SELECT` |
| Insert Data | Add new records | `INSERT` |
| Update Data | Modify existing records | `UPDATE` |
| Delete Data | Remove records | `DELETE` |
| Create Structures | Create tables/databases | `CREATE` |
| Remove Structures | Delete tables/databases | `DROP` |
| Manage Security | Control permissions | `GRANT` |
| Manage Transactions | Save/revert changes | `COMMIT` |

---

## Basic SQL Example

```sql
SELECT name
FROM students;
```

---

## Query Explanation

| SQL Part | Meaning |
|---|---|
| `SELECT` | Choose data |
| `name` | Select name column |
| `FROM students` | Read from students table |

---

## Output Example

| name |
|---|
| John |
| Sarah |

---

## Step-by-Step Workflow

```text
User Writes SQL Query
        ↓
Database Receives Query
        ↓
SQL Parser Checks Syntax
        ↓
Database Searches Data
        ↓
Results Returned To User
```

---

## Real-World Example

### Example: Shopee Order History

When users open order history:

SQL retrieves:

- order records
- payment details
- shipping information

---

### Example: Netflix

SQL retrieves:

- account information
- subscription plans
- watch history

---

> 💡 Beginner Note
>
> SQL is NOT the database itself.
>
> SQL is the language used to communicate with databases.

---

## Common Beginner Mistakes

| Mistake | Why It Is Wrong |
|---|---|
| Thinking SQL is a database | SQL is only a language |
| Thinking SQL only stores data | SQL also retrieves, updates, secures, and manages data |
| Thinking SQL is only for programmers | Analysts and engineers also use SQL |

---

## Key Takeaway

SQL is the standard language used to communicate with relational databases.

---

# 1.3 Why SQL is Important

SQL is one of the most valuable technical skills in modern technology.

Almost every industry stores structured data.

---

## Why Businesses Need SQL

| Industry | Data Stored |
|---|---|
| Banking | Transactions |
| Healthcare | Patient records |
| E-commerce | Orders |
| Education | Student records |
| Government | Citizen records |
| Social Media | User accounts |

---

## Why Developers Need SQL

Backend developers use SQL for:

- login systems
- payment systems
- APIs
- user accounts
- inventory systems

---

## Why Data Engineers Need SQL

Data engineers use SQL for:

- ETL pipelines
- ELT pipelines
- warehouse systems
- data transformations

---

## Why Analysts Need SQL

Analysts use SQL for:

- dashboards
- reports
- KPIs
- customer analysis

---

## Why ML Engineers Need SQL

Machine learning engineers use SQL for:

- data cleaning
- feature engineering
- dataset preparation

---

## Real-World Workflow Example

### Banking Transfer Example

Imagine transferring RM500 using a banking app.

---

### Workflow

```text
User Enters Transfer Amount
           ↓
Backend Receives Request
           ↓
SQL Query Executes
           ↓
Database Updates Balance
           ↓
Transfer Completed
```

---

### SQL Example

```sql
UPDATE accounts
SET balance = balance - 500
WHERE account_id = 101;
```

---

## Career Roles Using SQL

| Career Role | Why SQL Is Needed |
|---|---|
| Backend Engineer | Store application data |
| Data Analyst | Generate reports |
| Data Engineer | Build pipelines |
| DBA | Manage databases |
| ML Engineer | Prepare datasets |
| BI Developer | Create dashboards |

---

> 💡 Beginner Note
>
> Even if applications use ORM tools like:
>
> - Prisma
> - Hibernate
> - Django ORM
>
> SQL knowledge is still extremely important.

---

## Key Takeaway

SQL powers modern software systems and business operations.

---

# 1.4 SQL Use Cases

SQL is used in nearly every industry.

---

## E-Commerce Systems

SQL stores:

- products
- orders
- payments
- customers

Examples:

- Shopee
- Amazon
- Lazada

---

## Banking Systems

SQL stores:

- balances
- transfers
- transaction history

Examples:

- Maybank
- CIMB
- Public Bank

---

## Healthcare Systems

SQL stores:

- patient records
- appointments
- billing
- prescriptions

---

## Education Systems

SQL stores:

- student registration
- attendance
- grades

---

## Social Media Systems

SQL stores:

- users
- posts
- comments
- messages

Examples:

- Facebook
- Instagram

---

## Logistics Systems

SQL stores:

- deliveries
- drivers
- tracking records

Examples:

- Grab
- Foodpanda

---

## Example Query

```sql
SELECT *
FROM orders
WHERE customer_id = 1001;
```

---

## Query Explanation

| SQL Part | Meaning |
|---|---|
| `SELECT *` | Select all columns |
| `FROM orders` | Read from orders table |
| `WHERE customer_id = 1001` | Filter one customer |

---

## Key Takeaway

SQL exists in almost every major software system today.

---

# 1.5 SQL vs Programming Languages

Many beginners confuse SQL with programming languages.

They are different technologies with different purposes.

---

## SQL

SQL is a declarative language.

You tell the database:

> WHAT you want

Example:

```sql
SELECT name
FROM employees;
```

The database decides HOW to retrieve the data.

---

## Programming Languages

Examples:

- Python
- Java
- JavaScript
- C++

Programming languages tell the computer:

> HOW to perform tasks

Example:

```python
for employee in employees:
    print(employee.name)
```

---

## Comparison Table

| Feature | SQL | Programming Languages |
|---|---|---|
| Type | Declarative | Procedural/OOP |
| Focus | Data | Application Logic |
| Usage | Database operations | Application development |
| Example | SQL | Python |

---

## Real-World Workflow

```text
Frontend Receives User Input
             ↓
Backend Processes Logic
             ↓
SQL Retrieves Database Data
             ↓
Backend Returns Response
             ↓
Frontend Displays Result
```

---

## Key Takeaway

SQL manages data.

Programming languages build applications.

---

# 1.6 SQL vs NoSQL

Many beginners ask:

> Which is better?

Correct question:

> Which one fits the problem?

---

## SQL Databases

Examples:

- PostgreSQL
- MySQL
- Oracle
- SQL Server

Best for:

- banking
- ERP systems
- transactional systems

---

## NoSQL Databases

Examples:

- MongoDB
- Redis
- Cassandra
- DynamoDB

Best for:

- caching
- flexible documents
- distributed systems

---

## Comparison Table

| Feature | SQL | NoSQL |
|---|---|---|
| Schema | Fixed | Flexible |
| Relationships | Strong | Limited |
| Transactions | Strong ACID | Varies |
| Scaling | Vertical | Horizontal |

---

## Real Company Architecture Example

Modern companies often combine databases:

| Technology | Usage |
|---|---|
| PostgreSQL | Orders |
| Redis | Caching |
| MongoDB | Product Catalog |

---

> 💡 Beginner Note
>
> SQL and NoSQL are not enemies.
>
> Modern systems often use both together.

---

## Key Takeaway

Different databases solve different problems.

---

# 1.7 SQL in Modern Applications

SQL exists almost everywhere in modern systems.

---

## Streaming Platforms

Stores:

- subscriptions
- watch history
- payments

Example:

- Netflix

---

## Ride-Hailing Apps

Stores:

- riders
- drivers
- trip records

Example:

- Grab

---

## Banking Apps

Stores:

- balances
- transfers
- transactions

---

## Government Systems

Stores:

- tax records
- identity information
- licenses

---

## E-Commerce Apps

Stores:

- products
- orders
- payments

---

## Key Takeaway

Most applications rely on SQL somewhere in their architecture.

---

# 1.8 SQL for Backend Development

Backend developers use SQL constantly.

---

## What is Backend?

Backend is the system users cannot directly see.

---

## Frontend

Visible to users:

- buttons
- forms
- pages

---

## Backend

Handles:

- business logic
- authentication
- database communication

---

## Login Workflow Example

```text
User Enters Email/Password
              ↓
Backend Receives Request
              ↓
SQL Query Sent To Database
              ↓
Database Returns User Record
              ↓
Backend Verifies Password
              ↓
User Successfully Logs In
```

---

## SQL Example

```sql
SELECT *
FROM users
WHERE email = 'john@gmail.com';
```

---

## Backend Tools

| Language | ORM Tool |
|---|---|
| Python | Django ORM |
| Node.js | Prisma |
| Java | Hibernate |
| C# | Entity Framework |

---

## Key Takeaway

Backend systems constantly interact with SQL databases.

---

# 1.9 SQL for Data Engineering

Data engineers move and transform large amounts of data.

---

## Responsibilities

- move data
- clean data
- transform data
- build pipelines

---

## Example Workflow

```text
Application Generates Raw Data
               ↓
Data Engineer Extracts Data
               ↓
SQL Cleans/Transforms Data
               ↓
Data Loaded Into Warehouse
               ↓
Business Team Uses Reports
```

---

## SQL Example

```sql
INSERT INTO warehouse_sales
SELECT *
FROM app_sales;
```

---

## Common Tools

- Snowflake
- BigQuery
- Redshift
- dbt
- Airflow

---

## Key Takeaway

SQL is heavily used in data pipelines and warehousing systems.

---

# 1.10 SQL for Analytics

SQL is the primary language used in analytics.

---

## Business Questions SQL Helps Answer

- Which product sells most?
- Why did sales drop?
- Which customers spend most?
- Which marketing campaign performs best?

---

## SQL Example

```sql
SELECT SUM(revenue)
FROM orders;
```

---

## Output

Returns total company revenue.

---

## BI Tools

- Tableau
- Power BI
- Looker

---

## Key Takeaway

SQL helps businesses make data-driven decisions.

---

# 1.11 SQL for Machine Learning Pipelines

Many beginners think machine learning only uses Python.

That is incomplete.

SQL is heavily used before model training.

---

## Machine Learning Workflow

```text
Collect Raw Data
        ↓
Clean Data Using SQL
        ↓
Create Features
        ↓
Prepare Training Dataset
        ↓
Train Machine Learning Model
```

---

## SQL Example

```sql
SELECT customer_id,
       total_orders,
       total_spending
FROM customer_features;
```

---

## Real Use Cases

- fraud detection
- recommendation systems
- customer churn prediction

---

## Platforms

- BigQuery ML
- Snowflake
- Databricks

---

## Key Takeaway

SQL prepares clean structured data for machine learning systems.

---

# 1.12 Final Summary

After completing this section, beginners should understand:

- what SQL is
- why SQL matters
- where SQL is used
- how SQL works
- how SQL connects with applications
- how SQL supports analytics and machine learning

This foundation prepares learners for more advanced SQL topics later.
