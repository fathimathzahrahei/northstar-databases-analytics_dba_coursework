# NorthStar Urban Mobility And Logistics: Databases and Analytics Coursework
Module: Databases and Analytics (CP60056E)
Module Tutor: Dr Shaheen
Name: Fathimath Zahra
Student ID: 32146933
Batch: 2

# Overview
This repository contains the analytical work, code, database design, and
written report produced for the NorthStar Urban Mobility and Logistics case
study. The project investigates operational inefficiencies, customer-experience
failures, and data-architecture limitations affecting a multi-service urban
mobility provider, using an integrated stack of SQL within R, R analytics,
Python data processing, and MongoDB Atlas NoSQL design with query optimisation.

# Business Context
NorthStar Urban Mobility and Logistics operates passenger shuttle services, last-mile delivery warehouse dispatch, EV charging infrastructure, and a
mobile platform across several major UK cities. Despite rising demand,
operational performance has deteriorated: complaints are rising, delivery
windows are missed, and costs are growing faster than revenue. This project
applies database and analytics techniques to identify the root causes and
propose a redesigned data environment.

# Repository Structure
|----data/
|  |---raw/
|  |---cleaned/
|----notebooks/
|----report/
|----diagrams/
|----README.md

# Notebooks
|          Notebook           |                             Purpose                              |             Tools                |
|-----------------------------|------------------------------------------------------------------|----------------------------------|
|     `01_sql_in_r.ipynb`     | SQL queries within R - operational filtering, joins, aggregation |      R, RSQLite, sqldf           |
|     `02_r_analytics.ipynb`  | Statistical analysis and visualisation                           |      R, dplyr, ggplot2           |
| `03_python_processing.ipynb`| Cleaning pipeline, feature engineering, deeper analytics         |Python, pandas, numpy,matplotlib,          seaborn               | 
|   `04_mongodb_design.ipynb` | NoSQL schema design and CRUD operations on MongoDB Atlas         |        Python, PyMongo           | 
|`05_query_optimisation.ipynb`| Indexing strategy and explain-plan analysis                      |        Python, PyMongo           |


# Dataset
The NorthStar dataset comprises nine CSV files covering hubs, customers,
drivers, vehicles, orders, deliveries, incidents, complaints, and digital
platform events. A data dictionary is included. The dataset deliberately
contains inconsistent categorical values, missing values, cross-file
relationships, and hidden operational delay/failure patterns, reflecting
the case-study description of a fragmented data environment.

# Reproducibility
All notebooks read CSV files directly from the `data/raw/` folder via the
GitHub raw-content URL, so they execute end-to-end in Google Colab without
manual file uploads. Each notebook contains markdown cells explaining the
analytical purpose, the methodology, and the business interpretation of every
output.

# Methodology Reference
Case Study- NorthStar Urban Mobiliy and Logistics
