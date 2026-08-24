# PostgreSQL Database Administration

## L2/L3 Production DBA, HA, Performance, Migration & AWS Training

### Course Level

**Intermediate to Advanced | L2/L3 DBA | 100% Hands-On**

### Target Audience

* PostgreSQL Database Administrators
* Oracle DBAs transitioning to PostgreSQL
* Production Support Engineers
* Database Engineers
* Cloud DBAs
* DevOps / SRE Engineers supporting PostgreSQL
* Database Migration Engineers
* Technical professionals preparing for PostgreSQL production DBA roles

---

# Course Objectives

This program is designed to build **production-ready PostgreSQL Database Administrators** capable of installing, configuring, securing, monitoring, troubleshooting, tuning, backing up, recovering, replicating, upgrading, migrating, and operating PostgreSQL databases in enterprise environments.

The training covers:

* PostgreSQL internals and architecture
* Linux administration required for PostgreSQL DBAs
* Installation and configuration
* Database and object administration
* Security and access management
* Transactions, locking and concurrency
* VACUUM and autovacuum
* Backup, restore and disaster recovery
* Incremental backup
* Point-in-Time Recovery
* Streaming and logical replication
* High availability and automatic failover
* Patroni and repmgr
* PgBouncer and HAProxy
* Monitoring and troubleshooting
* Performance tuning
* Query optimization
* Index and partition management
* Major upgrades and patching
* Oracle-to-PostgreSQL migration
* AWS RDS for PostgreSQL
* Production incident handling
* Capacity planning and DBA automation

---

# Detailed Course Index

## Module 1 – PostgreSQL Introduction & DBA Fundamentals

### 1.1 PostgreSQL Overview

* History and evolution of PostgreSQL
* PostgreSQL architecture philosophy
* PostgreSQL vs Oracle
* PostgreSQL vs MySQL/MariaDB
* Open-source PostgreSQL ecosystem
* Community PostgreSQL vs managed PostgreSQL
* PostgreSQL release lifecycle
* Major vs minor releases

### 1.2 Role of a PostgreSQL DBA

* L1, L2 and L3 responsibilities
* Development vs testing vs production environments
* Production change management
* DBA operational responsibilities
* Incident, problem and change management
* SLA, RTO and RPO concepts
* Production DBA daily checklist

### Lab

* PostgreSQL environment introduction
* PostgreSQL documentation navigation
* DBA health-check exercise

---

# Module 2 – Linux Administration for PostgreSQL DBAs

## 2.1 Linux Fundamentals

* Linux filesystem structure
* Users and groups
* Ownership and permissions
* sudo
* Processes and signals
* Environment variables
* Shell profiles
* File management
* Network basics

## 2.2 Linux Monitoring

* top
* ps
* free
* vmstat
* iostat
* sar
* ss
* lsof
* df
* du

## 2.3 PostgreSQL OS Integration

* postgres OS account
* Environment variables
* PATH
* PGDATA
* PGHOST
* PGPORT
* PGDATABASE
* PGUSER
* Service management
* systemd
* Startup and shutdown automation

### Lab

* Build Linux PostgreSQL DBA environment
* Configure postgres account
* Configure environment variables
* OS resource monitoring

---

# Module 3 – PostgreSQL Installation & Initial Configuration

## 3.1 Package Installation

* YUM/DNF installation
* APT installation
* PostgreSQL repository configuration
* Package structure

## 3.2 Source Code Installation

* Required packages
* Downloading source
* configure
* make
* make install
* Custom installation directories

## 3.3 Cluster Initialization

* initdb
* Locale
* Encoding
* Authentication defaults
* Data checksums
* WAL directory considerations

## 3.4 PostgreSQL Service Management

* pg_ctl
* systemctl
* Start
* Stop
* Restart
* Reload
* Status
* Smart, fast and immediate shutdown

### Lab

* Install PostgreSQL using packages
* Compile PostgreSQL from source
* Create multiple PostgreSQL clusters
* Configure automatic startup

---

# Module 4 – PostgreSQL Architecture & Internals

## 4.1 PostgreSQL Process Architecture

* Postmaster/server process
* Backend processes
* Background processes
* Checkpointer
* Background writer
* WAL writer
* Autovacuum launcher/workers
* Archiver
* WAL sender
* WAL receiver
* Logical replication workers
* Parallel workers

## 4.2 Memory Architecture

* Shared memory
* shared_buffers
* WAL buffers
* work_mem
* maintenance_work_mem
* temp_buffers
* effective_cache_size

## 4.3 Storage Architecture

* Database cluster
* Database
* Tablespace
* Relation
* Fork
* Page/block
* Tuple
* TOAST
* FSM
* Visibility Map

## 4.4 MVCC Architecture

* Tuple versions
* xmin/xmax
* Visibility
* Dead tuples
* Transaction IDs
* MultiXact
* Transaction ID wraparound

## 4.5 WAL Architecture

* WAL records
* WAL segments
* LSN
* WAL buffers
* Checkpoints
* Crash recovery
* Full-page writes

### Lab

* Identify PostgreSQL processes
* Inspect database files
* Inspect relation files
* Map objects to physical files
* Observe WAL generation

---

# Module 5 – PostgreSQL Data Directory & Configuration

## 5.1 PGDATA Structure

* base
* global
* pg_wal
* pg_tblspc
* pg_stat
* pg_stat_tmp
* pg_replslot
* pg_logical
* pg_multixact
* pg_xact
* postmaster.pid

## 5.2 Configuration Files

* postgresql.conf
* postgresql.auto.conf
* pg_hba.conf
* pg_ident.conf

## 5.3 Configuration Management

* ALTER SYSTEM
* SHOW
* SET
* pg_settings
* Reload vs restart parameters
* Parameter context
* Configuration validation

### Lab

* Modify configuration safely
* ALTER SYSTEM exercise
* Reload/restart testing
* Troubleshoot invalid configuration

---

# Module 6 – PostgreSQL Client & Administration Tools

* psql
* pgAdmin
* DBeaver
* pg_isready
* createdb
* dropdb
* createuser
* dropuser
* vacuumdb
* reindexdb
* pg_config
* pg_controldata

## psql Advanced Usage

* Meta commands
* Variables
* Output formatting
* Script execution
* Timing
* Expanded display
* Connection management

### Lab

* Perform administration completely through psql
* Build reusable DBA scripts

---

# Module 7 – Database & Object Administration

## 7.1 Database Management

* CREATE DATABASE
* ALTER DATABASE
* DROP DATABASE
* Templates
* Database ownership
* Connection limits

## 7.2 Schema Management

* Schemas
* search_path
* Ownership
* Privileges

## 7.3 Object Management

* Tables
* Views
* Materialized views
* Sequences
* Identity columns
* Generated columns
* Functions
* Procedures
* Triggers
* Extensions

## 7.4 Data Types

* Numeric
* Character
* Date/time
* Boolean
* UUID
* Arrays
* JSON/JSONB
* Network types
* Range types

## 7.5 Constraints

* Primary key
* Foreign key
* Unique
* Check
* NOT NULL
* Exclusion constraints

### Lab

* Build an application database
* Create schemas and objects
* Object dependency analysis

---

# Module 8 – SQL for PostgreSQL DBAs

* SELECT
* INSERT
* UPDATE
* DELETE
* MERGE
* COPY
* Joins
* Subqueries
* CTEs
* Recursive queries
* Aggregate functions
* Window functions
* DDL
* DML
* DCL
* TCL

## DBA-Focused SQL

* PostgreSQL catalog queries
* information_schema
* pg_catalog
* Metadata extraction
* Database size queries
* Object size queries
* Session analysis queries

### Lab

* Develop a DBA SQL toolkit

---

# Module 9 – Users, Roles, Security & Authentication

## 9.1 Role Administration

* Users vs roles
* LOGIN/NOLOGIN
* SUPERUSER
* CREATEDB
* CREATEROLE
* REPLICATION
* Role inheritance
* Group roles

## 9.2 Privileges

* GRANT
* REVOKE
* Ownership
* Default privileges
* Schema permissions
* Function permissions
* Sequence permissions

## 9.3 Authentication

* pg_hba.conf
* Local
* Peer
* Password authentication
* SCRAM-SHA-256
* Certificate authentication
* LDAP concepts
* PAM concepts
* OAuth concepts
* pg_ident.conf

## 9.4 Transport Security

* SSL/TLS
* Certificates
* Client certificates

## 9.5 Row-Level Security

* RLS
* CREATE POLICY
* USING
* WITH CHECK
* Multi-tenant security patterns

## 9.6 Security Hardening

* Least privilege
* PUBLIC privileges
* Superuser control
* Secure search_path
* Password management
* Connection security
* Security audit checklist

### Lab

* Implement enterprise role hierarchy
* Configure SCRAM authentication
* Configure SSL
* Configure Row-Level Security

---

# Module 10 – Tablespaces & Physical Storage Management

* Tablespace architecture
* Creating tablespaces
* Moving objects
* Tablespace permissions
* Tablespace capacity monitoring
* Symbolic links
* Storage planning
* Tablespace backup/recovery considerations

### Lab

* Create multiple tablespaces
* Relocate tables and indexes
* Simulate storage pressure

---

# Module 11 – Transactions, MVCC, Locking & Concurrency

## 11.1 Transactions

* BEGIN
* COMMIT
* ROLLBACK
* SAVEPOINT

## 11.2 Isolation Levels

* Read Committed
* Repeatable Read
* Serializable

## 11.3 MVCC

* Snapshot management
* Tuple visibility
* Long-running transactions

## 11.4 Locks

* Table locks
* Row locks
* Advisory locks
* Lightweight locks concepts
* Blocking sessions
* Waiting sessions
* Deadlocks

### Lab

* Create blocking scenarios
* Detect blockers
* Resolve blocking
* Reproduce a deadlock
* Analyze long-running transactions

---

# Module 12 – VACUUM, Autovacuum & Database Maintenance

## 12.1 VACUUM

* VACUUM
* VACUUM ANALYZE
* VACUUM FULL
* Visibility Map
* Dead tuple cleanup

## 12.2 Autovacuum

* Autovacuum architecture
* autovacuum_vacuum_threshold
* autovacuum_vacuum_scale_factor
* autovacuum_analyze_threshold
* autovacuum_analyze_scale_factor
* Worker configuration
* Per-table tuning

## 12.3 Transaction ID Wraparound

* XID lifecycle
* Frozen tuples
* relfrozenxid
* datfrozenxid
* Emergency autovacuum

## 12.4 Bloat

* Table bloat
* Index bloat
* REINDEX
* REINDEX CONCURRENTLY
* pg_repack concepts

### Lab

* Generate dead tuples
* Observe autovacuum
* Tune autovacuum
* Analyze table/index bloat

---

# Module 13 – PostgreSQL Logging, Auditing & Housekeeping

## 13.1 Logging

* logging_collector
* log_destination
* log_directory
* log_filename
* log_rotation
* log_min_duration_statement
* log_statement
* log_lock_waits
* log_checkpoints
* log_connections
* log_disconnections
* CSV/JSON logging concepts

## 13.2 Audit

* Native logging
* pgaudit
* Audit design
* Security audit requirements

## 13.3 Log Analysis

* pgBadger
* Slow-query analysis
* Error pattern identification

## 13.4 Housekeeping

* Log retention
* WAL archive cleanup
* Temporary files
* Capacity checks

### Lab

* Configure production logging
* Generate pgBadger report
* Investigate a simulated incident from logs

---

# Module 14 – Backup & Restore Fundamentals

## 14.1 Backup Architecture

* RPO/RTO
* Logical vs physical backup
* Hot vs cold backup
* Full vs incremental strategy
* Backup retention
* Backup encryption considerations

## 14.2 Logical Backup

* pg_dump
* pg_dumpall
* Custom format
* Directory format
* Parallel backup
* Selective backup

## 14.3 Logical Restore

* psql restore
* pg_restore
* Parallel restore
* Object-level restore

## 14.4 Physical Backup

* pg_basebackup
* Backup manifests
* WAL inclusion
* Replication slots

## 14.5 Backup Validation

* pg_verifybackup
* Restore testing

### Lab

* Database backup and restore
* Schema-level restore
* Table-level restore
* Parallel backup/restore
* Physical base backup
* Backup verification

---

# Module 15 – WAL Archiving & Point-in-Time Recovery

## 15.1 WAL Archiving

* archive_mode
* archive_command
* archive_library concepts
* WAL retention
* Archive monitoring

## 15.2 PITR

* Recovery targets
* Time
* Transaction ID
* LSN
* Named restore point

## 15.3 Recovery Configuration

* restore_command
* recovery.signal
* recovery_target_time
* recovery_target_lsn
* recovery_target_name
* recovery_target_action

### Lab

**Production PITR Simulation**

1. Create database workload
2. Take base backup
3. Archive WAL
4. Accidentally delete data
5. Stop database
6. Restore backup
7. Replay WAL
8. Recover to immediately before deletion
9. Validate recovered data

---

# Module 16 – Incremental Backup & Advanced Backup Tools

## 16.1 PostgreSQL Native Incremental Backup

* Incremental backup architecture
* WAL summaries
* pg_basebackup incremental workflow
* Backup dependency chain
* pg_combinebackup
* Synthetic full backup
* pg_verifybackup
* Recovery testing

## 16.2 pgBackRest

* Architecture
* Repository
* Full backup
* Differential backup
* Incremental backup
* Retention
* Restore
* PITR
* Parallel backup
* Compression
* Encryption concepts

## 16.3 Barman

* Architecture
* Backup server design
* WAL streaming
* Retention
* Recovery

## 16.4 Automation

* Cron
* Backup scripts
* Monitoring failed backups
* Restore validation

### Lab

* Native incremental backup
* Combine backup chain
* Verify backup
* pgBackRest setup
* PITR using pgBackRest

---

# Module 17 – Streaming Replication

## 17.1 Physical Replication Architecture

* WAL sender
* WAL receiver
* Replication protocol
* Standby signal
* Hot standby

## 17.2 Replication Setup

* pg_basebackup
* primary_conninfo
* standby.signal
* Replication users
* Replication slots

## 17.3 Replication Modes

* Asynchronous
* Synchronous
* Quorum-based synchronous replication concepts

## 17.4 Advanced Replication

* Cascading replication
* Delayed standby
* Replication slots
* WAL retention

## 17.5 Monitoring

* pg_stat_replication
* pg_stat_wal_receiver
* Replay LSN
* Write/flush/replay lag

### Lab

* Build primary + standby
* Configure streaming replication
* Test synchronous replication
* Simulate replication lag

---

# Module 18 – Failover, Switchover & Disaster Recovery

* Planned switchover
* Unplanned failover
* Promotion
* Split-brain risks
* pg_promote()
* pg_ctl promote
* Timeline management
* Rejoining old primary
* pg_rewind
* DR site architecture
* RPO/RTO validation
* DR drills

### Lab

* Primary failure simulation
* Promote standby
* Redirect application
* Rewind old primary
* Rejoin cluster
* Planned switchover drill

---

# Module 19 – Logical Replication

## 19.1 Architecture

* Publisher
* Subscriber
* Publication
* Subscription
* Logical replication workers
* Replication slots

## 19.2 Configuration

* wal_level
* Publications
* Subscriptions
* Initial synchronization

## 19.3 Advanced Logical Replication

* Row filters
* Column lists
* Conflict handling
* Sequence considerations
* DDL considerations
* Logical replication security
* Monitoring
* Logical replication failover concepts
* Upgrade/migration use cases

## 19.4 Logical Decoding

* Replication slots
* Output plugins
* CDC concepts

### Lab

* Configure publisher/subscriber
* Replicate selected tables
* Implement row-filtered replication
* Monitor replication

---

# Module 20 – PostgreSQL High Availability with repmgr

* repmgr architecture
* repmgr metadata
* Primary registration
* Standby registration
* repmgrd
* Monitoring
* Switchover
* Failover
* Rejoin
* Witness server concepts
* Failure scenarios

### Lab

* Build repmgr cluster
* Perform switchover
* Simulate primary failure
* Rejoin failed node

---

# Module 21 – PostgreSQL High Availability with Patroni

* Patroni architecture
* Distributed configuration store
* etcd concepts
* Patroni REST API
* Bootstrap
* Cluster configuration
* Leader election
* Automatic failover
* Synchronous mode
* patronictl
* Node reinitialization
* Switchover
* Failover
* Split-brain prevention
* Watchdog concepts

### Lab

Build:

**PostgreSQL + Patroni + etcd HA Cluster**

Then perform:

* Leader failure
* Automatic failover
* Node rejoin
* Controlled switchover
* Application connectivity testing

---

# Module 22 – Connection Pooling & Load Balancing

## PgBouncer

* PgBouncer architecture
* Session pooling
* Transaction pooling
* Statement pooling
* Authentication
* Pool sizing
* Monitoring
* Prepared statement considerations

## HAProxy

* TCP load balancing
* Health checks
* Primary/replica routing
* Patroni integration

### Lab

Build:

**Application → HAProxy → PgBouncer → Patroni PostgreSQL Cluster**

Test application behavior during failover.

---

# Module 23 – PostgreSQL Monitoring & Observability

## 23.1 Core Statistics

* pg_stat_activity
* pg_stat_database
* pg_stat_user_tables
* pg_stat_all_tables
* pg_stat_user_indexes
* pg_statio_user_tables
* pg_stat_replication
* pg_stat_wal_receiver
* pg_stat_archiver
* pg_stat_bgwriter
* pg_stat_checkpointer
* pg_stat_wal
* pg_stat_io

## 23.2 Locks

* pg_locks
* Blocking trees
* Deadlock analysis

## 23.3 Progress Monitoring

* VACUUM
* ANALYZE
* CREATE INDEX
* COPY
* CLUSTER
* Base backup

## 23.4 Extensions/Tools

* pg_stat_statements
* pg_buffercache
* pg_activity
* pgBadger

## 23.5 Infrastructure Monitoring

* CPU
* Memory
* Disk
* IOPS
* Network
* Filesystem
* WAL generation
* Connection utilization

### Lab

* Build PostgreSQL DBA monitoring dashboard queries
* Diagnose CPU bottleneck
* Diagnose I/O bottleneck
* Diagnose blocking
* Diagnose connection exhaustion

---

# Module 24 – Query Performance Tuning

## 24.1 Query Planner

* Parser
* Rewriter
* Planner/optimizer
* Executor

## 24.2 EXPLAIN

* EXPLAIN
* EXPLAIN ANALYZE
* BUFFERS
* WAL
* VERBOSE
* FORMAT JSON

## 24.3 Scan Methods

* Sequential scan
* Index scan
* Index-only scan
* Bitmap scans

## 24.4 Join Algorithms

* Nested loop
* Hash join
* Merge join

## 24.5 Planner Statistics

* ANALYZE
* default_statistics_target
* Column statistics
* Extended statistics
* Cardinality estimation

## 24.6 Parallel Query

* Parallel sequential scan
* Parallel index scan
* Parallel joins
* Parallel aggregation
* Gather
* Gather Merge
* Worker configuration

## 24.7 JIT

* JIT architecture
* When JIT helps
* When JIT adds overhead

### Lab

* Analyze slow queries
* Compare execution plans
* Tune statistics
* Tune parallel execution

---

# Module 25 – PostgreSQL Indexing

## Index Types

* B-tree
* Hash
* GIN
* GiST
* SP-GiST
* BRIN

## Advanced Indexing

* Multicolumn indexes
* Covering indexes
* INCLUDE
* Partial indexes
* Expression indexes
* Unique indexes
* Index-only scans
* Operator classes
* Index selectivity

## Index Maintenance

* REINDEX
* REINDEX CONCURRENTLY
* Unused indexes
* Duplicate indexes
* Index bloat
* pg_amcheck

## Hypothetical Indexing

* hypopg

### Lab

* Design indexes for workload
* Identify unused indexes
* Create hypothetical indexes
* Measure query improvement

---

# Module 26 – Server & Memory Performance Tuning

## Memory

* shared_buffers
* work_mem
* maintenance_work_mem
* effective_cache_size
* huge_pages

## WAL

* wal_buffers
* checkpoint_timeout
* max_wal_size
* min_wal_size
* checkpoint_completion_target

## Connections

* max_connections
* Connection cost
* Pooling

## Planner

* random_page_cost
* seq_page_cost
* effective_io_concurrency
* Statistics tuning

## OS

* CPU
* RAM
* Swap
* Filesystem
* Storage latency
* IOPS
* HugePages
* Kernel considerations

## Modern PostgreSQL I/O

* PostgreSQL asynchronous I/O concepts
* I/O concurrency
* pg_stat_io-based analysis

### Lab

* Baseline database
* Tune parameters
* Benchmark before/after
* Analyze system impact

---

# Module 27 – pgbench & Performance Benchmarking

* pgbench architecture
* Initialization
* Built-in workloads
* Custom scripts
* TPS
* Latency
* Connection scaling
* Benchmark methodology
* Warm vs cold cache
* Avoiding misleading benchmarks

### Lab

* Generate workload
* Establish baseline
* Tune PostgreSQL
* Repeat benchmark
* Compare results

---

# Module 28 – Table Partitioning & Large Database Management

## Partitioning

* Range
* List
* Hash

## Partition Administration

* Partition pruning
* Partition-wise operations concepts
* ATTACH PARTITION
* DETACH PARTITION
* Partition indexes
* Partition maintenance
* Data retention using partitions

## Inheritance

* PostgreSQL inheritance
* Partitioning vs inheritance

## Large Database Strategies

* Archiving
* Retention
* Cold data
* Table design
* Index management

### Lab

* Build large partitioned table
* Load data
* Verify pruning
* Perform partition maintenance

---

# Module 29 – PostgreSQL Extensions & Advanced DBA Utilities

## Extensions

* pg_stat_statements
* pg_buffercache
* dblink
* postgres_fdw
* file_fdw concepts
* hypopg
* pg_trgm
* pgaudit

## Core DBA Utilities

* pg_amcheck
* pg_checksums
* pg_controldata
* pg_waldump
* pg_walsummary
* pg_archivecleanup
* pg_receivewal
* pg_verifybackup
* pg_combinebackup
* pg_rewind

### Lab

* Extension deployment
* Buffer cache inspection
* Integrity checks
* WAL inspection

---

# Module 30 – Data Integrity & Corruption Handling

* Data checksums
* Checksum verification
* pg_checksums
* pg_amcheck
* Backup verification
* Index corruption concepts
* Table corruption concepts
* Hardware/storage failure indicators
* WAL corruption considerations
* Recovery decision process

### Lab

* Enable/check data checksums
* Run pg_amcheck
* Validate backup integrity
* Practice corruption-response workflow

---

# Module 31 – PostgreSQL Upgrade & Patching

## Minor Version Upgrade

* PostgreSQL patching
* Pre-checks
* Backup
* Package upgrade
* Restart
* Validation
* Rollback planning

## Major Version Upgrade

* pg_dump/pg_restore
* pg_upgrade
* Link vs copy mode
* Extension compatibility
* Statistics
* Post-upgrade tasks

## Replication-Based Upgrade

* Logical replication migration
* Reduced-downtime upgrade strategies

### Lab

* Perform minor upgrade
* Perform pg_upgrade
* Run pre/post validation
* Practice rollback plan

---

# Module 32 – Oracle to PostgreSQL Migration

## 32.1 Assessment

* Oracle/PostgreSQL architecture differences
* Data type mapping
* Object compatibility
* SQL compatibility
* PL/SQL conversion considerations

## 32.2 Schema Migration

* Tables
* Constraints
* Sequences
* Indexes
* Views
* Procedures/functions

## 32.3 Migration Tools

* ora2pg
* pgloader where applicable
* AWS Schema Conversion Tool concepts
* AWS DMS

## 32.4 Data Migration

* Offline migration
* Online migration
* CDC
* Validation

## 32.5 Cutover

* Pre-cutover checklist
* Application freeze
* Final synchronization
* Validation
* DNS/application changes
* Rollback strategy

### Lab

* Oracle assessment
* Schema conversion
* Data migration
* Validation
* Cutover simulation

---

# Module 33 – AWS RDS for PostgreSQL

## AWS Fundamentals for DBAs

* Regions
* Availability Zones
* VPC
* Subnets
* Security Groups
* IAM concepts

## RDS Architecture

* DB instances
* Instance classes
* Storage
* Parameter groups
* Option concepts
* Maintenance windows

## RDS PostgreSQL Administration

* Creating RDS PostgreSQL
* Connectivity
* Parameter management
* Extensions
* Logs
* Monitoring

## Backup & Recovery

* Automated backups
* Manual snapshots
* Point-in-Time Restore
* Snapshot copy

## High Availability

* Multi-AZ
* Failover
* Read replicas
* Cross-region DR concepts

## Monitoring

* CloudWatch
* Enhanced Monitoring
* Performance Insights/Database Insights concepts

## Security

* Security Groups
* SSL
* IAM database authentication concepts
* Encryption
* KMS

## Migration

* AWS DMS
* Full load
* CDC
* Cutover

### Lab

* Provision PostgreSQL RDS
* Configure connectivity
* Configure parameter group
* Create snapshot
* PITR
* Configure replica
* Monitor workload

---

# Module 34 – Production Troubleshooting & Incident Management

## Common Production Incidents

* PostgreSQL not starting
* Database connection failure
* Too many connections
* Long-running queries
* Blocking
* Deadlocks
* High CPU
* High memory
* Swap usage
* High disk I/O
* Disk full
* WAL filesystem full
* Replication lag
* Replication broken
* Archive failure
* Backup failure
* Autovacuum issues
* Table/index bloat
* Slow queries
* Standby conflict
* Failed failover
* Corruption indicators

## Troubleshooting Methodology

1. Understand symptoms
2. Determine business impact
3. Collect evidence
4. Check database
5. Check OS
6. Check logs
7. Identify root cause
8. Apply recovery
9. Validate
10. Document RCA

### Lab

* Production incident war-room simulations

---

# Module 35 – Capacity Planning & Database Growth Management

* Database growth
* Table growth
* Index growth
* WAL growth
* Connection growth
* CPU capacity
* Memory capacity
* Storage capacity
* IOPS requirements
* Transaction workload
* Forecasting
* Alert thresholds
* Scaling vertically
* Scaling read workloads
* Archival strategies

### Lab

* Analyze historical growth
* Prepare 6/12-month capacity forecast

---

# Module 36 – DBA Automation & Scripting

## Shell Automation

* Health checks
* Backup scripts
* Log cleanup
* Disk monitoring
* Replication monitoring

## SQL Automation

* Metadata reports
* Database growth reports
* Blocking reports
* Bloat reports
* Backup validation

## Scheduling

* cron
* Job logging
* Error handling
* Alerting

### Lab

Build a **PostgreSQL Daily Health Check Framework**.

---

# Module 37 – Production Architecture & Best Practices

## Architecture Design

* Standalone PostgreSQL
* Primary/standby
* Multi-standby
* Cascading replicas
* HA cluster
* DR architecture
* Read scaling
* Connection pooling

## Production Standards

* Naming standards
* Security baseline
* Backup baseline
* Monitoring baseline
* Logging baseline
* Parameter baseline
* Capacity baseline
* Documentation standards

## Operational Documentation

* SOP
* Runbook
* Change plan
* Implementation plan
* Rollback plan
* RCA
* DR plan

---

# Module 38 – PostgreSQL 18 & Modern PostgreSQL Features for DBAs

* PostgreSQL release-management strategy
* Native incremental backup enhancements
* pg_combinebackup
* WAL summary files and pg_walsummary
* Logical replication enhancements
* Logical replication failover
* Modern monitoring statistics
* pg_stat_io
* Checkpointer statistics
* Data checksum improvements
* Modern pg_upgrade behavior
* Asynchronous I/O architecture
* OAuth authentication concepts
* Modern optimizer improvements
* Skip-scan concepts for multicolumn B-tree indexes
* Generated-column enhancements
* UUIDv7
* New DBA utilities and operational changes
* Version-specific feature compatibility

### Lab

* Compare supported PostgreSQL versions
* Test modern DBA features
* Build upgrade-readiness checklist

---

# Module 39 – PostgreSQL DBA Security & Compliance Workshop

* Production security assessment
* Role audit
* Privilege audit
* Authentication review
* pg_hba.conf audit
* SSL validation
* RLS validation
* Audit logging
* Database ownership
* PUBLIC permissions
* Unused accounts
* Password standards
* Extension security
* Backup security
* Security incident investigation

### Lab

Perform a **complete PostgreSQL production security audit** and produce remediation recommendations.

---

# Module 40 – Final Production Capstone Project

Students build and operate an enterprise PostgreSQL environment.

## Target Architecture

**Application**

↓

**HAProxy**

↓

**PgBouncer**

↓

**PostgreSQL HA Cluster**

* Primary
* Standby 1
* Standby 2
* Patroni
* etcd
* WAL Archive
* pgBackRest Repository
* Monitoring

## Capstone Activities

### Phase 1 – Build

* Linux configuration
* PostgreSQL installation
* Database configuration
* Security configuration
* Tablespaces
* Logging

### Phase 2 – HA

* Streaming replication
* Patroni
* Automatic failover
* HAProxy
* PgBouncer

### Phase 3 – Backup & DR

* Full backup
* Incremental backup
* WAL archive
* PITR
* Restore validation

### Phase 4 – Performance

* Generate pgbench workload
* Capture baseline
* Find slow queries
* Tune indexes
* Tune memory
* Tune autovacuum
* Compare results

### Phase 5 – Failure Simulation

Students troubleshoot:

* PostgreSQL crash
* Primary server failure
* Replica failure
* Replication lag
* Connection exhaustion
* Blocking
* Deadlock
* Disk full
* WAL archive failure
* Slow query
* Backup failure

### Phase 6 – DR

* Promote DR
* Validate data
* Restore primary
* Rejoin using pg_rewind
* Execute planned switchover

### Phase 7 – Documentation

Students prepare:

* Architecture document
* Installation SOP
* Backup SOP
* Restore SOP
* PITR SOP
* Failover SOP
* Switchover SOP
* Upgrade SOP
* Production health-check document
* Troubleshooting runbook
* DR runbook

---

# Recommended Tools Covered

| Category                  | Tools                                    |
| ------------------------- | ---------------------------------------- |
| PostgreSQL CLI            | psql, pg_ctl, pg_isready                 |
| GUI                       | pgAdmin, DBeaver                         |
| Backup                    | pg_dump, pg_restore, pg_basebackup       |
| Advanced Backup           | pgBackRest, Barman                       |
| Native Incremental Backup | pg_basebackup, pg_combinebackup          |
| Backup Validation         | pg_verifybackup                          |
| HA                        | Patroni, repmgr                          |
| Connection Pooling        | PgBouncer                                |
| Load Balancing            | HAProxy                                  |
| Monitoring                | pg_stat views, pg_activity               |
| Query Monitoring          | pg_stat_statements                       |
| Log Analysis              | pgBadger                                 |
| Benchmarking              | pgbench                                  |
| Integrity                 | pg_amcheck, pg_checksums                 |
| Recovery                  | pg_rewind                                |
| WAL                       | pg_waldump, pg_walsummary, pg_receivewal |
| Migration                 | ora2pg, pgloader, AWS DMS                |
| Index Analysis            | hypopg                                   |
| Cloud                     | AWS RDS PostgreSQL                       |

---

# Recommended Training Lab Architecture

For effective L2/L3 training, each student should ideally have:

* **Linux Server 1:** PostgreSQL Primary
* **Linux Server 2:** PostgreSQL Standby
* **Linux Server 3:** PostgreSQL Standby / DR
* **Linux Server 4:** Patroni/etcd/HA components where required
* Backup repository
* AWS account/lab environment
* Migration source database
* Load-generation environment

Recommended practice includes intentionally breaking the environment and requiring students to diagnose and recover it.

---

# Suggested Training Duration

| Track                                  | Suggested Duration |
| -------------------------------------- | -----------------: |
| PostgreSQL Fundamentals & Architecture |             3 Days |
| Core Administration                    |             4 Days |
| Security & Maintenance                 |             3 Days |
| Backup, Restore & PITR                 |             4 Days |
| Replication & DR                       |             4 Days |
| HA / Patroni / repmgr                  |             4 Days |
| Performance Tuning                     |             5 Days |
| Monitoring & Troubleshooting           |             3 Days |
| Upgrade & Migration                    |             3 Days |
| AWS RDS PostgreSQL                     |             3 Days |
| Capstone & Production Drills           |             4 Days |
| **Total Recommended Program**          |        **40 Days** |

For an intensive program, this can be compressed to approximately **25–30 training days**, but for genuine L2/L3 hands-on capability, the longer lab-focused format is preferable.

---

# Training Methodology

Recommended delivery model:

**30% Concepts + 70% Hands-On Labs**

Every major topic should follow:

**Architecture → Configuration → Validation → Failure → Troubleshooting → Recovery → Production Best Practices**

For example:

**Streaming Replication**

Architecture
↓
Configure Primary
↓
Build Standby
↓
Validate Replication
↓
Generate Replication Lag
↓
Break Replication
↓
Troubleshoot
↓
Failover
↓
Rebuild/Rejoin
↓
Production Best Practices

This approach develops production DBAs rather than only teaching PostgreSQL commands.

---

# Student Assessment

## Weekly Assessments

* Architecture questions
* DBA SQL exercises
* Troubleshooting scenarios
* Configuration exercises

## Practical Assessments

Students must independently perform:

* PostgreSQL installation
* Backup and restore
* PITR
* Replication setup
* Failover
* Switchover
* pg_rewind
* Patroni setup
* Performance troubleshooting
* Security configuration
* Major upgrade
* Migration
* AWS RDS administration

## Final Assessment

Students receive a broken production-like PostgreSQL environment and must:

1. Identify the incident.
2. Determine impact.
3. Troubleshoot it.
4. Restore service.
5. Validate data.
6. Find root cause.
7. Recommend preventive action.
8. Produce an RCA.

---

# Expected Outcome

After completing this program, students should be able to independently perform **L2/L3 PostgreSQL DBA responsibilities**, including:

* Install and configure production PostgreSQL
* Administer databases, roles and objects
* Secure PostgreSQL environments
* Manage VACUUM and autovacuum
* Implement enterprise backup strategies
* Perform complete and point-in-time recovery
* Configure physical and logical replication
* Perform failover and switchover
* Build HA PostgreSQL environments
* Configure Patroni, repmgr, PgBouncer and HAProxy
* Monitor database and operating-system health
* Troubleshoot production incidents
* Tune SQL and PostgreSQL configuration
* Manage indexes and partitioned databases
* Perform PostgreSQL upgrades
* Detect integrity and corruption issues
* Migrate Oracle workloads to PostgreSQL
* Administer PostgreSQL on AWS RDS
* Design backup, HA and DR strategies
* Automate routine DBA activities
* Create production SOPs, runbooks and RCA documents

The final objective is to move the learner from **“knowing PostgreSQL” to being able to own a PostgreSQL production environment.**

[1]: https://www.postgresql.org/docs/current/index.htm "PostgreSQL: Documentation: 18: PostgreSQL 18.6 Documentation"
