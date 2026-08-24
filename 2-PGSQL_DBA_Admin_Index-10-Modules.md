# PostgreSQL DBA Training – 10 Module Detailed Index

## Module 1: PostgreSQL Fundamentals, Linux, Architecture & Installation

* PostgreSQL History, Introduction & Ecosystem
* PostgreSQL vs Oracle, MySQL and Other Databases
* PostgreSQL Versions, Releases & Support Lifecycle
* Role and Responsibilities of PostgreSQL DBA – L1/L2/L3
* Linux Setup and Basic Administration

  * Filesystem Structure
  * Users, Groups & Permissions
  * Processes & Services
  * CPU, Memory & Disk Basics
  * Network Basics
* PostgreSQL Environment Variables

  * `PGDATA`
  * `PGHOST`
  * `PGPORT`
  * `PGDATABASE`
  * `PGUSER`
  * `PATH`
* PostgreSQL Installation

  * YUM/DNF Installation
  * APT Installation
  * Source Code Compilation
* Cluster Initialization with `initdb`
* PostgreSQL Startup & Shutdown

  * `pg_ctl`
  * `systemctl`
  * Smart, Fast & Immediate Shutdown
* PostgreSQL Architecture

  * Client/Server Architecture
  * Postmaster Process
  * Backend Processes
  * Background Writer
  * Checkpointer
  * WAL Writer
  * Autovacuum Workers
  * Archiver
  * WAL Sender & Receiver
* PostgreSQL Memory Architecture

  * Shared Buffers
  * WAL Buffers
  * Work Memory
  * Maintenance Work Memory
* PostgreSQL Physical Architecture

  * Database Cluster
  * Database
  * Tablespace
  * Relation Files
  * Pages & Tuples
  * TOAST
  * FSM & Visibility Map
* PostgreSQL Data Directory Structure

  * `base`
  * `global`
  * `pg_wal`
  * `pg_tblspc`
  * `pg_xact`
  * `pg_replslot`
* PostgreSQL Configuration Files

  * `postgresql.conf`
  * `postgresql.auto.conf`
  * `pg_hba.conf`
  * `pg_ident.conf`
* `ALTER SYSTEM`, `SHOW`, `SET` & `pg_settings`

**Hands-On:** Linux setup, package installation, source installation, `initdb`, cluster creation, configuration and architecture validation.

---

## Module 2: Core PostgreSQL Database Administration

* PostgreSQL Client & Administration Tools

  * `psql`
  * pgAdmin
  * DBeaver
* Advanced `psql` Commands
* Database Creation & Management
* Database Templates
* Schema Management
* `search_path`
* PostgreSQL Object Flow
* Tables & Temporary Tables
* Views & Materialized Views
* Sequences & Identity Columns
* Functions & Procedures
* Triggers
* Extensions
* Data Types

  * Numeric
  * Character
  * Date/Time
  * Boolean
  * UUID
  * Arrays
  * JSON/JSONB
* Constraints

  * Primary Key
  * Foreign Key
  * Unique
  * Check
  * NOT NULL
* SQL Operations

  * DDL
  * DML
  * DCL
  * TCL
* PostgreSQL Joins

  * Inner Join
  * Left/Right Join
  * Full Join
  * Cross Join
* CTEs & Subqueries
* COPY Command
* Data Export & Import
* PostgreSQL Metadata & System Catalogs

  * `pg_catalog`
  * `information_schema`
* Tablespace Management

  * Create/Alter/Drop Tablespaces
  * Moving Objects
  * Tablespace Capacity Management
* Database & Object Size Monitoring
* Object Dependency Management

**Hands-On:** Create a complete application database with schemas, tablespaces, tables, constraints, views, indexes, sequences and application objects.

---

## Module 3: Security, Transactions, MVCC & Database Maintenance

* PostgreSQL Users & Roles
* LOGIN & NOLOGIN Roles
* SUPERUSER
* CREATEDB
* CREATEROLE
* REPLICATION Role
* Role Membership & Inheritance
* GRANT & REVOKE
* Object Ownership
* Default Privileges
* Host-Based Authentication
* `pg_hba.conf`
* `pg_ident.conf`
* Authentication Methods

  * Peer
  * Password
  * SCRAM-SHA-256
  * Certificate
  * LDAP/PAM Concepts
* SSL/TLS Configuration
* Row-Level Security
* Policy Creation

  * `CREATE POLICY`
  * `USING`
  * `WITH CHECK`
* Security Hardening & Least Privilege
* PostgreSQL Transactions

  * BEGIN
  * COMMIT
  * ROLLBACK
  * SAVEPOINT
* Transaction Isolation Levels

  * Read Committed
  * Repeatable Read
  * Serializable
* MVCC Architecture
* Tuple Visibility
* Transaction IDs
* XID Wraparound
* PostgreSQL Locks

  * Table Locks
  * Row Locks
  * Advisory Locks
* Blocking Sessions
* Waiting Sessions
* Deadlocks
* VACUUM
* VACUUM FULL
* ANALYZE
* Autovacuum Architecture
* Autovacuum Configuration & Tuning
* Dead Tuple Management
* Table & Index Bloat
* REINDEX & REINDEX CONCURRENTLY
* PostgreSQL Logging

  * Slow Query Logging
  * Connection Logging
  * Checkpoint Logging
  * Lock-Wait Logging
* Audit Logging
* pgAudit
* Log Rotation & Housekeeping

**Hands-On:** Configure enterprise security, create RLS policies, simulate locks/deadlocks, troubleshoot blocking and tune autovacuum.

---

## Module 4: Backup, Restore, PITR & Disaster Recovery

* Backup & Recovery Architecture
* RPO & RTO
* Logical vs Physical Backups
* Logical Backup

  * `pg_dump`
  * `pg_dumpall`
* Logical Restore

  * `psql`
  * `pg_restore`
* Backup Formats

  * Plain
  * Custom
  * Directory
* Parallel Backup & Restore
* Database-Level Backup
* Schema-Level Backup
* Table-Level Backup
* Physical Backup
* `pg_basebackup`
* Backup Manifest
* `pg_verifybackup`
* WAL Architecture
* WAL Segments
* LSN
* WAL Archiving

  * `archive_mode`
  * `archive_command`
* Point-in-Time Recovery

  * Time-Based Recovery
  * LSN-Based Recovery
  * Named Restore Points
* `restore_command`
* `recovery.signal`
* Native Incremental Backup
* WAL Summaries
* `pg_combinebackup`
* pgBackRest

  * Full Backup
  * Differential Backup
  * Incremental Backup
  * Retention
  * Restore
  * PITR
* Barman
* Backup Automation with Cron
* Backup Monitoring
* Backup Validation
* Disaster Recovery Planning
* Restore Testing & DR Drills

**Hands-On:** Perform logical/physical backups, intentionally delete production-like data, and recover it using PITR and pgBackRest.

---

## Module 5: Replication, High Availability & Automatic Failover

* PostgreSQL Replication Architecture
* Physical Streaming Replication
* Primary & Standby Configuration
* Hot Standby
* `standby.signal`
* `primary_conninfo`
* WAL Sender & WAL Receiver
* Replication Slots
* Asynchronous Replication
* Synchronous Replication
* Quorum-Based Replication Concepts
* Cascading Replication
* Delayed Standby
* Replication Monitoring

  * `pg_stat_replication`
  * `pg_stat_wal_receiver`
* Replication Lag

  * Write Lag
  * Flush Lag
  * Replay Lag
* Manual Failover
* Standby Promotion
* Planned Switchover
* Timeline Management
* Split-Brain Scenarios
* `pg_rewind`
* Rejoining Failed Primary
* Logical Replication

  * Publisher
  * Subscriber
  * Publication
  * Subscription
  * Row Filters
  * Column Lists
  * Logical Replication Slots
* Logical Decoding & CDC Concepts
* repmgr

  * Installation
  * Node Registration
  * repmgrd
  * Switchover
  * Failover
  * Rejoin
* Patroni

  * Architecture
  * etcd
  * Leader Election
  * Automatic Failover
  * `patronictl`
  * Switchover
  * Failover
* PgBouncer

  * Session Pooling
  * Transaction Pooling
  * Pool Sizing
* HAProxy

  * Health Checks
  * Primary/Replica Routing
* HA & DR Architecture Design

**Hands-On:** Build a multi-node PostgreSQL HA cluster using streaming replication, Patroni, etcd, PgBouncer and HAProxy; perform failover and switchover drills.

---

## Module 6: PostgreSQL Performance Tuning & Query Optimization

* PostgreSQL Performance Tuning Methodology
* Performance Baseline
* Query Planner & Optimizer
* `EXPLAIN`
* `EXPLAIN ANALYZE`
* `BUFFERS`
* `WAL`
* Query Execution Plans
* Sequential Scan
* Index Scan
* Index-Only Scan
* Bitmap Scan
* Join Algorithms

  * Nested Loop
  * Hash Join
  * Merge Join
* PostgreSQL Index Types

  * B-tree
  * Hash
  * GIN
  * GiST
  * SP-GiST
  * BRIN
* Multicolumn Indexes
* Covering Indexes
* Partial Indexes
* Expression Indexes
* Index Selectivity
* Unused & Duplicate Indexes
* `hypopg`
* Planner Statistics
* ANALYZE
* Extended Statistics
* Cardinality Estimation
* Parallel Query
* Gather & Gather Merge
* JIT Concepts
* Memory Tuning

  * `shared_buffers`
  * `work_mem`
  * `maintenance_work_mem`
  * `effective_cache_size`
* WAL & Checkpoint Tuning
* Connection Tuning

  * `max_connections`
  * PgBouncer
* Autovacuum Performance Tuning
* OS-Level Tuning

  * CPU
  * Memory
  * Swap
  * HugePages
  * Filesystem
  * IOPS
* `pg_stat_statements`
* Slow Query Analysis
* `pgbench`
* Benchmarking & Performance Baselines

**Hands-On:** Generate workload with pgbench, identify bottlenecks, optimize SQL/indexes/configuration and compare before/after performance.

---

## Module 7: Monitoring, Troubleshooting & Capacity Planning

* PostgreSQL Monitoring Architecture
* `pg_stat_activity`
* `pg_stat_database`
* `pg_stat_user_tables`
* `pg_stat_user_indexes`
* `pg_statio_user_tables`
* `pg_stat_replication`
* `pg_stat_wal_receiver`
* `pg_stat_archiver`
* `pg_stat_bgwriter`
* `pg_stat_checkpointer`
* `pg_stat_wal`
* `pg_stat_io`
* `pg_locks`
* Progress Monitoring
* `pg_stat_progress_vacuum`
* `pg_stat_progress_create_index`
* `pg_stat_progress_copy`
* `pg_stat_progress_basebackup`
* `pg_stat_statements`
* `pg_buffercache`
* pg_activity
* pgBadger
* OS Monitoring

  * top
  * vmstat
  * iostat
  * sar
  * free
  * df
  * du
* CPU Troubleshooting
* Memory Troubleshooting
* Disk I/O Troubleshooting
* Connection Exhaustion
* Slow Queries
* Blocking & Deadlocks
* Replication Lag
* Broken Replication
* Archive Failures
* Backup Failures
* Disk Full
* WAL Growth
* Autovacuum Issues
* Database Growth Monitoring
* Table & Index Growth
* Capacity Forecasting
* Alert Thresholds
* Daily DBA Health Checks
* Root Cause Analysis

**Hands-On:** Production war-room exercises covering CPU spikes, blocking, connection exhaustion, disk-full situations, replication lag and failed backups.

---

## Module 8: Partitioning, Integrity, Upgrades & Advanced Administration

* PostgreSQL Table Partitioning
* Range Partitioning
* List Partitioning
* Hash Partitioning
* Partition Pruning
* Partition Indexes
* ATTACH PARTITION
* DETACH PARTITION
* Partition Maintenance
* Data Retention Using Partitions
* PostgreSQL Table Inheritance
* Large Database Management
* PostgreSQL Extensions

  * `pg_stat_statements`
  * `pg_buffercache`
  * `dblink`
  * `postgres_fdw`
  * `hypopg`
  * `pg_trgm`
* Data Checksums
* `pg_checksums`
* `pg_amcheck`
* Corruption Detection
* Backup Integrity Checks
* WAL Inspection

  * `pg_waldump`
  * `pg_walsummary`
* Minor Version Upgrade & Patching
* Major Version Upgrade
* `pg_upgrade`
* Pre-Upgrade Checks
* Post-Upgrade Validation
* Extension Compatibility
* Upgrade Rollback Strategy
* Logical Replication-Based Upgrade
* PostgreSQL 18 DBA Features
* Native Incremental Backup Enhancements
* Asynchronous I/O Concepts
* Modern Monitoring Improvements
* Logical Replication Enhancements
* UUIDv7 & Modern SQL Features

**Hands-On:** Partition large tables, run integrity checks, patch PostgreSQL and perform a complete major-version upgrade.

---

## Module 9: Oracle to PostgreSQL Migration & AWS RDS PostgreSQL

### Oracle to PostgreSQL Migration

* Migration Assessment
* Oracle vs PostgreSQL Architecture
* Object Compatibility
* Data Type Mapping
* SQL Compatibility
* PL/SQL Conversion Considerations
* Schema Conversion
* Tables
* Constraints
* Sequences
* Indexes
* Views
* Functions & Procedures
* ora2pg
* pgloader
* AWS Schema Conversion Concepts
* AWS DMS
* Offline Migration
* Online Migration
* CDC
* Data Validation
* Object Validation
* Performance Validation
* Migration Cutover
* Rollback Planning

### AWS RDS for PostgreSQL

* AWS Basics for DBAs
* Regions & Availability Zones
* VPC & Subnets
* Security Groups
* RDS PostgreSQL Architecture
* DB Instance Classes
* Storage Configuration
* Parameter Groups
* PostgreSQL Extensions on RDS
* Automated Backups
* Manual Snapshots
* Point-in-Time Restore
* Multi-AZ
* Read Replicas
* Cross-Region DR Concepts
* CloudWatch
* Enhanced Monitoring
* Database Insights / Performance Monitoring
* SSL
* IAM Authentication Concepts
* Encryption & KMS
* AWS DMS Migration
* RDS Upgrade & Maintenance
* RDS Troubleshooting

**Hands-On:** Perform Oracle-to-PostgreSQL migration exercises and build/manage an AWS RDS PostgreSQL environment.

---

## Module 10: Production Operations, Automation & Final Capstone

### Production DBA Operations

* Daily DBA Activities
* Weekly & Monthly Maintenance
* Production Health Checks
* Change Management
* Incident Management
* Problem Management
* SLA Management
* RPO/RTO Validation

### DBA Automation

* Shell Scripting
* SQL Automation
* Cron Scheduling
* Backup Automation
* Database Health Check Scripts
* Replication Monitoring Scripts
* Database Growth Reports
* Blocking Reports
* Bloat Reports
* Log Cleanup
* WAL Archive Housekeeping

### Production Architecture

* Standalone PostgreSQL
* Primary/Standby
* Multi-Standby
* Cascading Replication
* HA Cluster
* DR Site
* Read Scaling
* Connection Pooling
* Backup Repository Architecture

### Production Documentation

* SOP
* Runbook
* Implementation Plan
* Change Plan
* Rollback Plan
* Backup & Recovery SOP
* PITR SOP
* Failover SOP
* Switchover SOP
* Upgrade SOP
* DR Runbook
* Root Cause Analysis (RCA)

### Final Capstone Project

Build an enterprise-style architecture:

**Application → HAProxy → PgBouncer → Patroni → PostgreSQL Primary/Standbys → pgBackRest Backup Repository**

Students perform:

* PostgreSQL Installation
* Production Configuration
* Security Hardening
* Streaming Replication
* Patroni HA Configuration
* Automatic Failover
* PgBouncer Connection Pooling
* HAProxy Load Balancing
* Backup Configuration
* Incremental Backup
* WAL Archiving
* PITR
* Performance Testing
* Query Tuning
* Autovacuum Tuning
* Monitoring
* Primary Failure Simulation
* Replication Failure
* Disk-Full Scenario
* Connection Exhaustion
* Blocking & Deadlock Troubleshooting
* Backup Failure
* DR Promotion
* `pg_rewind`
* Planned Switchover
* Production Documentation

**Final Goal:** Build the skills required to independently manage, troubleshoot, tune, secure and recover a production PostgreSQL environment as an **L2/L3 PostgreSQL DBA**.

---

## Core Hands-On Technology Stack

`PostgreSQL` • `Linux` • `psql` • `pgAdmin` • `pgBackRest` • `Barman` • `Patroni` • `repmgr` • `etcd` • `PgBouncer` • `HAProxy` • `pgBadger` • `pg_activity` • `pgbench` • `pg_stat_statements` • `pg_amcheck` • `pg_rewind` • `ora2pg` • `pgloader` • `AWS DMS` • `AWS RDS PostgreSQL`
