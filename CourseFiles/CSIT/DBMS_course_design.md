# Database Management Systems (DBMS)
**Target Program:** Bachelor of Technology (B.Tech)  
**Academic Credits:** 3 Credits  
**Core Activity Hours:** 20 Learning Hours

---

## I. Core Curricular Targets (COs & CSOs)

### Course Outcomes (COs)
* **CO-1:** Formulate conceptual data models using Entity-Relationship (ER) and Extended ER (EER) diagrams to capture complex real-world requirements.
* **CO-2:** Apply mathematical principles of functional dependencies and normalization algorithms (up to 3NF/BCNF) to design anomaly-free relational database schemas.
* **CO-3:** Construct efficient structured queries using relational algebra and advanced SQL operations to retrieve and manipulate datasets.
* **CO-4:** Evaluate database execution plans using profiling tools and implement strategic indexing methodologies to optimize query performance.
* **CO-5:** Analyze transaction states, schedules, and implement isolation levels to ensure data integrity and mitigate concurrency anomalies.
* **CO-6:** Differentiate between relational (SQL) and non-relational (NoSQL) database architectures to design hybrid data storage systems.

### Course Specific Outcomes (CSOs)
* **CSO-1:** Design, normalize, and program robust, production-grade backends for distributed enterprise applications ensuring relational integrity and absolute ACID compliance.
* **CSO-2:** Perform high-level database administration tasks, including query optimization profiling, physical schema tuning via indexing, and handling concurrent transaction deadlocks.
* **CSO-3:** Architect polyglot persistence layers utilizing both SQL engines and modern NoSQL stores to balance consistency and scale requirements in cloud computing ecosystems.

---

## II. The 45-Activity Structural Matrix

| Module Name | # | Activity Name | Format | Brief Execution Plan & Task | Tools Used | Mapped CO |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Unit 1: Intro & Data Modeling** | 1 | App Deconstruction | Team | Reverse-engineer data requirements of an application (e.g., Netflix) directly from its active UI screens. | Miro, MS Word | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 2 | Mini-ERD Speed Dating | Individual | Given a 3-sentence business rule, draw an ERD snapshot within a strict 7-minute limit. | Pen & Paper | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 3 | Cardinality War | Pair | One student presents a scenario; the other must prove why it's 1:M or M:N using real counterexamples. | Whiteboard | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 4 | Weak Entity Rescue | Individual | Convert a broken, disconnected dataset by designing a proper Weak Entity with an identifying relationship. | Draw.io | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 5 | ISA Hierarchy Refactoring | Team | Reorganize an e-commerce user structure using Specialization and Generalization (Disjoint vs. Overlapping). | Lucidchart | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 6 | Ambiguous Schema Challenge | Class | Analyze a purposely flawed enterprise description to identify and resolve structural design ambiguities. | Discussion | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 7 | Metadata Dictionary Blueprint | Individual | Construct a data dictionary defining constraints, types, and default keys for a library system. | MS Excel | **CO-1** |
| **Unit 1: Intro & Data Modeling** | 8 | File System vs. DBMS Crash Test | Individual | Write a Python script updating concurrent rows in a text file to witness data inconsistency firsthand. | Python CLI | **CO-1** |
| **Unit 2: Relational Model & Algebra** | 9 | Relational Algebra Translators | Individual | Convert a set of complex English queries into formal Relational Algebra expressions ($\sigma, \pi, \bowtie$). | Pen & Paper | **CO-3** |
| **Unit 2: Relational Model & Algebra** | 10 | Relational Domain Detective | Pair | Identify structural domain constraint violations within a corrupted data table provided by the instructor. | MS Excel | **CO-2** |
| **Unit 2: Relational Model & Algebra** | 11 | Tuple Calculus Matchmaking | Individual | Map Relational Algebra expressions directly to equivalent Tuple Relational Calculus (TRC) queries. | LaTeX Editor | **CO-3** |
| **Unit 2: Relational Model & Algebra** | 12 | Referential Integrity Break-In | Individual | Attempt to violate `ON DELETE CASCADE` and `SET NULL` configurations to log system verification behaviors. | SQLite / MySQL | **CO-2** |
| **Unit 2: Relational Model & Algebra** | 13 | Outer Join Paradox | Pair | Compute manual truth tables showing the structural differences between Left, Right, and Full Outer Joins. | Whiteboard | **CO-3** |
| **Unit 2: Relational Model & Algebra** | 14 | Division Operator Challenge | Individual | Write complex relational expressions to solve the "Find customers who ordered *all* products" problem. | Pen & Paper | **CO-3** |
| **Unit 3: Normalization Theory** | 15 | Closure Finder Race | Class | Given a relation schema and a set of FDs, compute the attribute closure ($X^+$) fastest. | Kahoot | **CO-2** |
| **Unit 3: Normalization Theory** | 16 | 1NF/2NF Unraveling | Individual | Take a multi-valued raw spreadsheet and normalize it step-by-step into First and Second Normal Forms. | Google Sheets | **CO-2** |
| **Unit 3: Normalization Theory** | 17 | 3NF Decomposition Clinic | Pair | Find and eliminate transitive dependencies from a messy real estate dataset. | Draw.io | **CO-2** |
| **Unit 3: Normalization Theory** | 18 | BCNF Conflict Resolution | Team | Decompose a table where a non-key determines a part of a composite key into BCNF relations. | Miro | **CO-2** |
| **Unit 3: Normalization Theory** | 19 | Lossless Join Verification | Individual | Apply Chase Method algorithms to mathematically prove if a schema decomposition is lossless. | Pen & Paper | **CO-2** |
| **Unit 3: Normalization Theory** | 20 | Dependency Preservation Audit | Individual | Verify whether all original functional dependencies can be checked within the decomposed tables. | Pen & Paper | **CO-2** |
| **Unit 3: Normalization Theory** | 21 | Denormalization Case Study | Team | Analyze a high-frequency read-heavy analytics system and strategically introduce redundancy for speed. | Markdown | **CO-2** |
| **Unit 4: Structured Query Language** | 22 | DDL Schema Deployment | Individual | Write and execute a complete SQL script defining tables, check constraints, and foreign key rules. | DBeaver, MySQL | **CO-3** |
| **Unit 4: Structured Query Language** | 23 | SQL Murder Mystery | Individual | Solve a gamified open-source interactive puzzle using advanced multi-table joins and subqueries. | Web Browser | **CO-3** |
| **Unit 4: Structured Query Language** | 24 | Group By / Having Deep Dive | Pair | Write analytical queries extracting regional revenue metrics while filtering aggregated groups. | PostgreSQL | **CO-3** |
| **Unit 4: Structured Query Language** | 25 | Nested vs. Correlated Subqueries | Individual | Rewrite a slow nested subquery into an efficient correlated subquery utilizing the `EXISTS` operator. | LiveSQL | **CO-3** |
| **Unit 4: Structured Query Language** | 26 | View Security Sandbox | Individual | Create a read-only Virtual View restricting a HR table to mask sensitive financial fields from users. | Oracle DB | **CO-3** |
| **Unit 4: Structured Query Language** | 27 | Trigger-Based Audit Logging | Individual | Write an `AFTER UPDATE` trigger that automatically logs old and new cell modifications into a history table. | PostgreSQL | **CO-3** |
| **Unit 4: Structured Query Language** | 28 | Stored Procedure Payroll System | Team | Build a programmable PL/SQL routine that calculates worker bonuses based on performance metrics. | SQL Developer | **CO-3** |
| **Unit 5: Storage & Indexing** | 29 | B+ Tree Visualizer | Individual | Step-by-step draw the insertion and splitting mechanism of a B+ Tree index given a continuous key sequence. | Pen & Paper | **CO-4** |
| **Unit 5: Storage & Indexing** | 30 | EXPLAIN Plan Deconstruction | Pair | Execute `EXPLAIN ANALYZE` on a query to identify bottlenecks like full table sequential scans. | pgAdmin | **CO-4** |
| **Unit 5: Storage & Indexing** | 31 | Indexing Speed Test | Individual | Generate 1 Million mock rows; measure read speed variance before and after creating a Composite B-Tree index. | Python, Postgres | **CO-4** |
| **Unit 5: Storage & Indexing** | 32 | Clustered vs. Non-Clustered Audit | Individual | Compare the physical storage footprints and lookup performance times between clustered and secondary indexes. | MS SQL Server | **CO-4** |
| **Unit 5: Storage & Indexing** | 33 | Query Rewrite Competition | Team | Take a highly unoptimized SQL query containing multiple `OR` statements and optimize it for a 10x speedup. | DBeaver | **CO-4** |
| **Unit 5: Storage & Indexing** | 34 | Dense vs. Sparse Index Mapping | Individual | Sketch block pointer structures for dense and sparse indexing to compare disk I/O operational tradeoffs. | Whiteboard | **CO-4** |
| **Unit 6: Transactions & Concurrency** | 35 | ACID Violation Simulation | Pair | Code a script that intentionally breaks the Atomicity property to inspect incomplete data states. | Python, SQLite | **CO-5** |
| **Unit 6: Transactions & Concurrency** | 36 | Conflict Serializability Checker | Individual | Construct a precedence graph for an interleaved transaction schedule to find if it is conflict-serializable. | Pen & Paper | **CO-5** |
| **Unit 6: Transactions & Concurrency** | 37 | Two-Phase Locking (2PL) Game | Pair | Manually simulate shared/exclusive lock requests between competing sessions to verify 2PL rules. | Terminal CLI | **CO-5** |
| **Unit 6: Transactions & Concurrency** | 38 | Deadlock Induction | Individual | Open two parallel terminal windows and execute commands to deliberately force a database deadlock state. | MySQL / Postgres | **CO-5** |
| **Unit 6: Transactions & Concurrency** | 39 | Isolation Level Experiment | Team | Change isolation settings from `Read Uncommitted` to `Serializable` to track Dirty Reads and Phantom Reads. | DBeaver CLI | **CO-5** |
| **Unit 6: Transactions & Concurrency** | 40 | Write-Ahead Logging (WAL) Audit | Individual | Trace a database engine's recovery log to simulate system crash recovery using UNDO/REDO operations. | Text Log | **CO-5** |
| **Unit 7: NoSQL & Capstone Application** | 41 | CAP Theorem Debate | Class | Debate the trade-offs between Availability and Consistency during network partitions in distributed databases. | Oral | **CO-6** |
| **Unit 7: NoSQL & Capstone Application** | 42 | NoSQL Document Store Setup | Individual | Convert a normalized 3NF relational user schema into an optimized, nested JSON document model. | MongoDB | **CO-6** |
| **Unit 7: NoSQL & Capstone Application** | 43 | Redis Caching Blueprint | Pair | Integrate a key-value caching layer to store transient session tokens, minimizing heavy primary DB lookups. | Redis, Node.js | **CO-6** |
| **Unit 7: NoSQL & Capstone Application** | 44 | Sharding & Replication Lab | Team | Configure a distributed cluster featuring one primary node and two read-replicas to test load horizontal scaling. | Docker, MongoDB | **CO-6** |
| **Unit 7: NoSQL & Capstone Application** | 45 | Master Capstone Showcase | Team | **Full-Stack Project:** Design, normalize, index, optimize, and deploy a secure full-stack database application. | Full Dev Stack | **CO-1 to CO-6** |
