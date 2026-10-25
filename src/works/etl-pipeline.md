---
title: ETL Pipeline with Airflow
order: 6
featured: false
year: 2025
category: Data Engineering
stack: Python, Apache Airflow, PostgreSQL, Docker
thumbLabel: Airflow · PostgreSQL
summary: My first serious project — an extract, transform and load pipeline written in Python, orchestrated with Apache Airflow and loading into PostgreSQL.
repo: https://github.com/00-Shreyas-00/ETL_project_personal
---

## Pipeline

### Extract, transform, load

An Airflow DAG runs three tasks in sequence. Extract fetches data and saves it to a run-specific working directory, transform reshapes it, and load writes the result to PostgreSQL with psycopg2 before cleaning up the temporary files.

## Setup

### Docker Compose and tests

Docker Compose runs PostgreSQL 13 and Apache Airflow 2.9, and each pipeline step has its own unit tests.
