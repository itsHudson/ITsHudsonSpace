# Section 20: Modifying Data

## 20.1 Data Modification Fundamentals
- What data modification means
- CRUD operations
- Transaction awareness
- Data integrity risks
- Production safety mindset

---

## 20.2 INSERT Basics
- Single-row insert
- Multi-row insert
- Explicit column insert
- Full row insert

---

## 20.3 INSERT INTO SELECT
- Copying data between tables
- Migration inserts
- Backup inserts

---

## 20.4 Bulk Inserts
- Batch inserts
- Bulk loading
- CSV imports
- High-volume ingestion

---

## 20.5 Default Value Inserts
- Auto-generated defaults
- NULL handling
- System-generated timestamps

---

## 20.6 Identity & Sequence Inserts
- AUTO_INCREMENT
- SERIAL
- IDENTITY
- SEQUENCE-generated values

---

## 20.7 INSERT Validation
- Constraint validation
- Foreign key validation
- Duplicate prevention

---

## 20.8 UPDATE Basics
- Single-row updates
- Multi-row updates
- Column updates

---

## 20.9 UPDATE with WHERE
- Safe updates
- Preventing accidental mass updates

---

## 20.10 UPDATE with JOIN
- Multi-table updates
- Joined updates

---

## 20.11 UPDATE with Subqueries
- Dynamic updates
- Conditional updates

---

## 20.12 Conditional Updates
- CASE-based updates
- Business rule updates

---

## 20.13 DELETE Basics
- Single-row deletes
- Multi-row deletes
- Conditional deletes

---

## 20.14 DELETE with WHERE
- Safe deletion strategies
- Preventing full-table deletes

---

## 20.15 DELETE with JOIN
- Multi-table deletes
- Relational cleanup

---

## 20.16 DELETE with Subqueries
- Conditional deletion logic

---

## 20.17 Soft Deletes
- Soft delete flags
- Archive strategies
- Recovery workflows

---

## 20.18 Hard Deletes
- Permanent deletion
- Irreversible removal risks

---

## 20.19 TRUNCATE vs DELETE
- Performance differences
- Logging differences
- Recovery differences

---

## 20.20 MERGE Statements
- MERGE basics
- Matched records
- Non-matched records

---

## 20.21 UPSERT Operations
- INSERT ON CONFLICT
- INSERT IGNORE
- REPLACE INTO
- ON DUPLICATE KEY UPDATE

---

## 20.22 Data Synchronization
- Source-to-target syncing
- Incremental sync workflows

---

## 20.23 Batch Processing
- Large updates
- Chunked modifications
- Scheduled modifications

---

## 20.24 Auditing Data Changes
- Audit logs
- Change tracking
- Before/after snapshots

---

## 20.25 Rollback Strategies
- Transaction rollback
- Savepoints
- Recovery planning

---

## 20.26 Locking During Modifications
- Row locks
- Table locks
- Deadlock risks

---

## 20.27 Concurrency Issues
- Lost updates
- Race conditions
- Concurrent writes

---

## 20.28 Performance Considerations
- Large batch updates
- Index impact
- Write amplification

---

## 20.29 Partitioned Table Modifications
- Updating partitioned tables
- Deleting partition data

---

## 20.30 Data Migration Modifications
- Legacy migration updates
- Data transformation updates

---

## 20.31 Security Considerations
- Update permissions
- Delete permissions
- Role restrictions

---

## 20.32 Debugging Data Modifications
- Missing WHERE clauses
- Incorrect joins
- Duplicate inserts

---

## 20.33 Vendor Differences
- MERGE support differences
- UPSERT syntax differences

---

## 20.34 Modification Anti-Patterns
- Full table updates
- Full table deletes
- Missing transactions
- Unsafe migration scripts

---

## 20.35 Real-World Modification Examples
- Order processing
- Payroll updates
- Inventory updates
- User profile updates
- Financial transaction systems

---
