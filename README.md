# claude-cc-skill-clickhouse-io-skill

A Claude Code skill for designing, querying, and optimizing ClickHouse databases for analytical workloads.

## Overview

ClickHouse is a column-oriented database designed for high-performance analytical queries. This skill focuses on table engines, data modeling, query design, ingestion, aggregation, and performance optimization.

## Main Capabilities

- Design tables for analytical access patterns.
- Choose suitable MergeTree-family engines.
- Select sorting and partitioning keys.
- Model data for filtering and aggregation.
- Optimize SQL queries.
- Use materialized views and projections where appropriate.
- Manage ingestion and data transformations.
- Work with distributed tables and clusters.
- Diagnose slow queries and resource usage.
- Apply data engineering best practices.

## When to Use It

Use this skill when designing ClickHouse schemas, building analytical pipelines, optimizing queries, reviewing data models, or troubleshooting performance.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-cc-skill-clickhouse-io-skill.git ~/.claude/skills/cc-skill-clickhouse-io
```

## Usage

Invoke the skill for ClickHouse development tasks:

```text
/cc-skill-clickhouse-io
```

Provide the ClickHouse version, table schema, query workload, data volume, ingestion pattern, and performance objective.

## Table Design Workflow

1. Identify the primary analytical queries.
2. Define the data model and row granularity.
3. Select an appropriate table engine.
4. Choose ordering and partitioning based on access patterns.
5. Define data types and compression choices.
6. Plan ingestion and deduplication behavior.
7. Add materialized views where they provide measurable value.
8. Validate query plans and execution metrics.
9. Review storage and maintenance requirements.

## Query Optimization

- Filter early using suitable columns.
- Avoid unnecessary wide scans.
- Select only required columns.
- Use aggregations that match the data model.
- Review join cardinality and execution behavior.
- Use materialized views for repeated expensive workloads when appropriate.
- Measure query performance with representative data.

## Data Engineering Checklist

- Table engine matches write and query patterns.
- Sorting key supports common filters.
- Partitioning is not excessively granular.
- Data types are appropriate.
- Retention and TTL behavior are defined.
- Ingestion is monitored.
- Duplicate handling is understood.
- Query performance is measured.
- Backups and recovery are considered.

## Repository Contents

- `SKILL.md`: Main ClickHouse analytics and engineering patterns.
- `README.md`: Table design, query workflow, and optimization guidance.

## Practical Principle

ClickHouse performance depends heavily on table design and query patterns. Tune the data model against real workloads rather than applying generic partitioning or indexing rules.
