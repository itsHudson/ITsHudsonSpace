# 1.1 SQL Fundamentals

---

## 1.1.1 What is SQL

---

### 1.1.1.1 Definition of SQL

---

SQL stands for:

| Term | Meaning |
|---|---|
| S | Structured |
| Q | Query |
| L | Language |

SQL is a specialized language used to:

- Store data
- Retrieve data
- Manage data
- Modify data
- Organize relational databases
- Control database access
- Perform analytics on data

SQL is mainly used with:

- Relational Database Management Systems (RDBMS)
- Data warehouses
- Analytical databases
- Cloud databases
- Enterprise systems

---

### 1.1.1.2 What is a Database

---

A database is an organized collection of data stored electronically.

Real-world examples:

| System | Stored Data |
|---|---|
| Banking System | Customer accounts, transactions |
| E-Commerce Website | Products, orders, users |
| Hospital System | Patients, doctors, appointments |
| School System | Students, courses, grades |
| Social Media | Posts, likes, comments |

Without databases:

- Data becomes messy
- Searching becomes difficult
- Updating information becomes slow
- Systems cannot scale properly

---

### 1.1.1.3 What is a Relational Database

---

A relational database stores data in tables.

Example:

#### Table: users

| user_id | name | email |
|---|---|---|
| 1 | Alice | alice@email.com |
| 2 | Bob | bob@email.com |

Each table contains:

| Component | Meaning |
|---|---|
| Row | One record |
| Column | One field |
| Table | Collection of related records |

Relationships connect tables together.

Example:

- Users table
- Orders table
- Payments table

A user can have many orders.

---

### 1.1.1.4 Basic SQL Example

---

Example SQL query:

```sql
SELECT name, email
FROM users
WHERE user_id = 1;
```

Explanation:

| SQL Part | Purpose |
|---|---|
| SELECT | Choose columns |
| FROM | Choose table |
| WHERE | Apply condition |

Result:

| name | email |
|---|---|
| Alice | alice@email.com |

---

### 1.1.1.5 What SQL Can Do

---

SQL can perform many operations.

| Category | Example |
|---|---|
| Create data | INSERT |
| Read data | SELECT |
| Update data | UPDATE |
| Delete data | DELETE |
| Create tables | CREATE TABLE |
| Modify tables | ALTER TABLE |
| Manage permissions | GRANT |
| Control transactions | COMMIT |

---

### 1.1.1.6 Real-World Analogy

---

Think of a database like a library.

| Library Component | Database Equivalent |
|---|---|
| Library | Database |
| Bookshelf | Table |
| Book | Row |
| Book title | Column |
| Librarian | Database administrator |
| Searching books | SQL query |

SQL acts like instructions given to the librarian.

Example:

- "Find all books written by John"
- "Show books published after 2020"
- "Delete damaged books"

This is similar to SQL queries.

---

### 1.1.1.7 Beginner Mistakes

---

| Mistake | Explanation |
|---|---|
| Thinking SQL is a full programming language | SQL mainly focuses on data operations |
| Confusing database with table | A database contains multiple tables |
| Thinking SQL only stores data | SQL also analyzes and manages data |
| Ignoring relationships | Relational databases depend heavily on relationships |

---

## 1.1.2 Why SQL is Important

---

### 1.1.2.1 SQL Powers Modern Systems

---

Almost every modern application uses SQL somewhere.

Examples:

| Industry | SQL Usage |
|---|---|
| Banking | Transactions |
| E-Commerce | Orders and inventory |
| Healthcare | Patient records |
| Social Media | Posts and comments |
| Logistics | Shipment tracking |
| Education | Student systems |

SQL is one of the most widely used technologies in the world.

---

### 1.1.2.2 SQL Handles Massive Data

---

Large companies store huge amounts of data.

Examples:

| Company Type | Example Data |
|---|---|
| E-Commerce | Millions of orders |
| Social Media | Billions of posts |
| Banking | Financial transactions |
| Streaming Services | Watch history |

SQL databases are designed to:

- Organize large datasets
- Retrieve data efficiently
- Handle concurrent users
- Maintain data consistency

---

### 1.1.2.3 SQL is Essential for Business Operations

---

Businesses depend on SQL for:

| Business Area | SQL Usage |
|---|---|
| Finance | Revenue tracking |
| Marketing | Customer analytics |
| Operations | Inventory management |
| HR | Employee systems |
| Security | User authentication |

Without SQL:

- Reports become inaccurate
- Systems become unreliable
- Business decisions become difficult

---

### 1.1.2.4 SQL is a Universal Skill

---

SQL is used by many roles.

| Role | Why SQL is Needed |
|---|---|
| Backend Developer | Store application data |
| Data Analyst | Analyze business data |
| Data Engineer | Build pipelines |
| DBA | Manage databases |
| BI Developer | Build dashboards |
| ML Engineer | Prepare datasets |

SQL is considered one of the most valuable technical skills.

---

### 1.1.2.5 SQL is Easy to Learn

---

Compared to many programming languages:

| Technology | Difficulty |
|---|---|
| SQL | Beginner-friendly |
| C++ | Complex |
| Java | Moderate |
| Assembly | Very difficult |

SQL syntax is readable.

Example:

```sql
SELECT * FROM products;
```

This is close to human language.

---

## 1.1.3 SQL Use Cases

---

### 1.1.3.1 Application Data Storage

---

Applications store user data using SQL.

Examples:

| Application | Stored Data |
|---|---|
| Facebook | Users, posts |
| Shopee | Orders, products |
| Banking App | Accounts, transfers |
| Food Delivery App | Restaurants, drivers |

---

### 1.1.3.2 Reporting and Analytics

---

Businesses generate reports using SQL.

Examples:

| Report Type | SQL Usage |
|---|---|
| Monthly sales | Revenue aggregation |
| Customer trends | User analysis |
| Inventory reports | Stock tracking |
| Financial reports | Profit calculation |

---

### 1.1.3.3 Authentication Systems

---

SQL databases store:

- User accounts
- Password hashes
- Roles
- Permissions

Example table:

| user_id | username | role |
|---|---|---|
| 1 | admin | administrator |

---

### 1.1.3.4 Transaction Systems

---

SQL is heavily used in transactions.

Examples:

| System | Transaction Type |
|---|---|
| ATM | Money withdrawal |
| E-Commerce | Payment processing |
| Airline Booking | Ticket reservation |

Transactions ensure:

- Accuracy
- Reliability
- Data consistency

---

### 1.1.3.5 Data Warehousing

---

Companies collect historical data for analysis.

SQL is used to:

- Aggregate data
- Build dashboards
- Create KPIs
- Generate insights

---

## 1.1.4 SQL vs Programming Languages

---

### 1.1.4.1 Main Difference

---

| SQL | Programming Languages |
|---|---|
| Focuses on data | Focuses on application logic |
| Declarative | Procedural/Object-oriented |
| Queries databases | Builds software |
| Asks WHAT to retrieve | Explains HOW to execute |

---

### 1.1.4.2 SQL is Declarative

---

In SQL:

You describe:

- What you want

You usually do not describe:

- Step-by-step execution process

Example:

```sql
SELECT * FROM employees;
```

You ask for data.

The database engine decides:

- How to retrieve it efficiently

---

### 1.1.4.3 Programming Languages are Procedural

---

Languages like:

- Python
- Java
- C++
- JavaScript

Usually involve:

- Variables
- Loops
- Functions
- Algorithms
- Memory management

Example in Python:

```python
for employee in employees:
    print(employee)
```

This explicitly defines execution flow.

---

### 1.1.4.4 SQL and Programming Languages Work Together

---

Modern systems combine both.

Example architecture:

| Component | Technology |
|---|---|
| Frontend | React |
| Backend | Node.js |
| Database | PostgreSQL |
| Query Language | SQL |

Workflow:

1. User clicks button
2. Backend receives request
3. Backend sends SQL query
4. Database returns result
5. Backend sends response to frontend

---

## 1.1.5 SQL vs NoSQL

---

### 1.1.5.1 SQL Databases

---

SQL databases use:

- Tables
- Rows
- Columns
- Relationships

Examples:

| SQL Database |
|---|
| MySQL |
| PostgreSQL |
| Oracle |
| SQL Server |

---

### 1.1.5.2 NoSQL Databases

---

NoSQL databases use flexible structures.

Examples:

| NoSQL Type | Example |
|---|---|
| Document DB | MongoDB |
| Key-Value DB | Redis |
| Column DB | Cassandra |
| Graph DB | Neo4j |

---

### 1.1.5.3 Core Differences

---

| Feature | SQL | NoSQL |
|---|---|---|
| Structure | Fixed schema | Flexible schema |
| Relationships | Strong relationships | Often weaker relationships |
| Scalability | Vertical scaling | Horizontal scaling |
| Consistency | Strong consistency | Flexible consistency |
| Query Language | SQL | Database-specific |

---

### 1.1.5.4 When SQL is Better

---

SQL is better for:

| Scenario | Reason |
|---|---|
| Banking | Strong consistency |
| Transactions | ACID support |
| Reporting | Complex joins |
| Structured systems | Organized schema |

---

### 1.1.5.5 When NoSQL is Better

---

NoSQL is useful for:

| Scenario | Reason |
|---|---|
| Real-time caching | Fast retrieval |
| Flexible documents | Dynamic structure |
| Massive scaling | Distributed systems |
| Event logging | High write throughput |

---

## 1.1.6 SQL in Modern Applications

---

### 1.1.6.1 SQL is Everywhere

---

Modern applications heavily rely on SQL.

Examples:

| Application Type | SQL Usage |
|---|---|
| Mobile apps | User data |
| Websites | Product catalog |
| SaaS platforms | Subscription systems |
| Enterprise systems | Internal operations |

---

### 1.1.6.2 Modern Architectures

---

SQL works with:

- Microservices
- APIs
- Cloud systems
- Containerized applications
- Kubernetes
- Serverless applications

---

### 1.1.6.3 SQL in Cloud Computing

---

Cloud providers offer managed SQL services.

Examples:

| Cloud Provider | SQL Service |
|---|---|
| AWS | RDS |
| Google Cloud | Cloud SQL |
| Azure | Azure SQL |
| Snowflake | Cloud warehouse |

Benefits:

- Automatic backups
- Scalability
- Security
- High availability

---

## 1.1.7 SQL for Backend Development

---

### 1.1.7.1 Backend Systems Depend on SQL

---

Backend developers use SQL to:

- Store users
- Manage authentication
- Process orders
- Save application data

---

### 1.1.7.2 Common Backend Workflow

---

Typical flow:

1. User submits request
2. Backend validates request
3. Backend executes SQL query
4. Database returns data
5. Backend returns API response

---

### 1.1.7.3 Example Backend Query

---

```sql
SELECT *
FROM orders
WHERE customer_id = 1001;
```

This retrieves customer orders.

---

## 1.1.8 SQL for Data Engineering

---

### 1.1.8.1 What is Data Engineering

---

Data engineering focuses on:

- Moving data
- Cleaning data
- Transforming data
- Building pipelines

---

### 1.1.8.2 SQL in ETL Pipelines

---

ETL means:

| Term | Meaning |
|---|---|
| E | Extract |
| T | Transform |
| L | Load |

SQL is heavily used during transformation.

Example:

```sql
SELECT
    customer_id,
    SUM(total_amount) AS total_sales
FROM orders
GROUP BY customer_id;
```

---

### 1.1.8.3 Data Warehouse Processing

---

Data engineers use SQL for:

- Aggregation
- Data cleaning
- Data normalization
- Reporting datasets

---

## 1.1.9 SQL for Analytics

---

### 1.1.9.1 SQL is Core to Analytics

---

Analysts use SQL to:

- Analyze trends
- Build reports
- Generate KPIs
- Create dashboards

---

### 1.1.9.2 Example Analytical Query

---

```sql
SELECT
    product_category,
    SUM(sales) AS total_sales
FROM sales_data
GROUP BY product_category;
```

This calculates total sales by category.

---

### 1.1.9.3 BI Tools Using SQL

---

| Tool | SQL Usage |
|---|---|
| Power BI | Data retrieval |
| Tableau | Dashboard queries |
| Looker | Analytical modeling |
| Metabase | Reporting |

---

## 1.1.10 SQL for Machine Learning Pipelines

---

### 1.1.10.1 SQL Prepares ML Data

---

Machine learning requires clean datasets.

SQL helps:

- Filter data
- Aggregate features
- Remove duplicates
- Handle missing values

---

### 1.1.10.2 Typical ML Data Pipeline

---

Workflow:

1. Raw data collected
2. SQL cleans data
3. Features are generated
4. Dataset exported
5. ML model training starts

---

### 1.1.10.3 Example Feature Engineering Query

---

```sql
SELECT
    customer_id,
    COUNT(order_id) AS total_orders,
    SUM(total_amount) AS lifetime_value
FROM orders
GROUP BY customer_id;
```

This creates ML features.

---

### 1.1.10.4 SQL + Python Workflow

---

Modern ML systems often combine:

| Purpose | Technology |
|---|---|
| Data extraction | SQL |
| Model training | Python |
| Visualization | Python |
| Storage | SQL databases |

---

### 1.1.10.5 Beginner Mistakes in ML SQL

---

| Mistake | Problem |
|---|---|
| Ignoring missing values | Poor model quality |
| Using dirty data | Incorrect predictions |
| Forgetting normalization | Model instability |
| Duplicate records | Biased training |

---
