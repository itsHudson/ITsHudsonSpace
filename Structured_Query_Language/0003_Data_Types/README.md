# Section 3: Data Types

## 3.1 Numeric Types

### Integer Types
- TINYINT
- SMALLINT
- MEDIUMINT
- INT
- BIGINT

### Exact Numeric Types
- DECIMAL
- NUMERIC
- MONEY
- SMALLMONEY

### Approximate Numeric Types
- FLOAT
- REAL
- DOUBLE PRECISION

### Auto Generated Numeric Types
- SERIAL
- BIGSERIAL
- IDENTITY

---

## 3.2 Numeric Precision & Scale
- Precision
- Scale
- Overflow
- Underflow
- Rounding behavior
- Decimal storage tradeoffs

---

## 3.3 String Types

### Fixed Length Strings
- CHAR
- NCHAR

### Variable Length Strings
- VARCHAR
- NVARCHAR

### Large Text Storage
- TEXT
- CLOB
- LONGTEXT

### Character Encoding
- ASCII
- UTF-8
- UTF-16
- Collation
- Case sensitivity

---

## 3.4 Boolean Types
- BOOLEAN
- BIT
- TRUE/FALSE handling
- Vendor-specific boolean behavior

---

## 3.5 Date & Time Types

### Date Types
- DATE

### Time Types
- TIME

### Combined Types
- DATETIME
- TIMESTAMP

### Extended Time Types
- TIMESTAMP WITH TIME ZONE
- TIMESTAMP WITHOUT TIME ZONE
- INTERVAL

### Time Concepts
- Epoch time
- Timezone conversion
- Daylight saving issues

---

## 3.6 Binary Types
- BINARY
- VARBINARY
- BLOB
- BYTEA
- IMAGE

---

## 3.7 UUID Types
- UUID
- GUID
- UUID generation
- UUID performance tradeoffs

---

## 3.8 JSON Types

### Basic JSON
- JSON storage
- JSON validation

### Advanced JSON
- JSONB
- Nested JSON
- JSON indexing
- JSON querying

---

## 3.9 XML Types
- XML storage
- XML parsing
- XPath
- XQuery

---

## 3.10 ENUM Types
- ENUM
- SET
- Lookup table alternative

---

## 3.11 Array Types
- Single-dimensional arrays
- Multi-dimensional arrays
- Array querying
- Array indexing

---

## 3.12 Spatial Data Types

### Geographic Types
- GEOGRAPHY

### Geometry Types
- GEOMETRY
- POINT
- LINESTRING
- POLYGON

### GIS Functions
- Distance calculation
- Spatial indexing

---

## 3.13 Document Types
- BSON
- XML documents
- JSON documents

---

## 3.14 Object Identifier Types
- ROWID
- Object identifiers
- Internal record identifiers

---

## 3.15 Large Object Types
- CLOB
- BLOB
- NCLOB
- File storage references

---

## 3.16 Specialized Vendor Types

### PostgreSQL
- HSTORE
- CIDR
- INET
- MACADDR
- TSVECTOR

### Oracle
- RAW
- LONG RAW

### SQL Server
- SQL_VARIANT
- HIERARCHYID

### BigQuery
- STRUCT
- ARRAY

---

## 3.17 NULL Handling
- NULL values
- NULL storage
- NULL comparisons
- Three-valued logic

---

## 3.18 Type Conversion
- CAST
- CONVERT
- Implicit conversion
- Explicit conversion
- Type coercion errors

---

## 3.19 Data Type Constraints
- Length restrictions
- Precision restrictions
- Allowed ranges
- Validation rules

---

## 3.20 Storage Optimization by Type
- Choosing efficient types
- Storage overhead
- Compression impact
- Performance implications

---

## 3.21 Data Serialization Formats
- JSON serialization
- XML serialization
- Binary serialization
- Avro basics
- Parquet basics

---

## 3.22 Data Type Best Practices
- Choose smallest valid type
- Avoid unnecessary TEXT usage
- Avoid floating point mistakes
- Use proper date types
- Normalize enum usage

---
