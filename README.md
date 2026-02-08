# Banking-Operations-Risk-Analytics-System

📌 Project Overview
This project focuses on the end-to-end analysis of banking data, consolidating over 30 years of financial records (1995–2026) to monitor loan distribution and customer risk. It transitions raw financial data through a Python-based ETL pipeline into a PostgreSQL database, culminating in a high-performance Power BI dashboard for executive decision-making.

🛠️ Tech Stack
Data Engineering: Python (Pandas, SQLAlchemy)

Database Management: PostgreSQL

Analysis: SQL (CTEs, Window Functions, Joins)

Visualization: Power BI (Advanced DAX)

Environment: Jupyter Notebook / VS Code

🚀 Key Features
1. Financial ETL Pipeline (Python)
Extraction: Automated ingestion of diverse banking datasets including loan balances, customer demographics, and transaction frequencies.

Transformation: * Standardized disparate financial columns for uniform SQL schema mapping.

Handled data types to ensure precision in monetary calculations (e.g., Bank Loans vs. Credit Card Balances).

Loading: Engineered a secure connection via SQLAlchemy to push cleaned data snapshots into a centralized PostgreSQL instance.

2. Advanced SQL Queries
Developed a suite of analytical scripts to answer critical business questions:

Risk Assessment: Segmented customers into "New," "Returning," and "Loyal" based on lifetime previous purchases and loan history.

Revenue Contribution: Calculated the percentage of total bank revenue contributed by specific age groups (e.g., Adult vs. Senior).

Exposure Analysis: Aggregated total debt across Bank, Business, and Credit Card sectors to identify high-risk accounts.

3. Power BI Dashboard & DAX Logic
Built a standalone dashboard that maintains analytical integrity across varying timeframes:

Dynamic Totals: Created custom DAX measures to sum complex loan types across multiple categories.

Filter Override: Implemented CALCULATE and ALL functions to ensure "Grand Total" cards display the full 1995–2026 dataset even when a specific year slicer (e.g., 2015+) is active.

Cross-Visual Interactions: Configured visual relationships to allow for deep-dives into customer segments without losing site of global KPIs.

📊 Business Insights

Risk Segments: Mapped the age groups responsible for the highest revenue contribution, allowing for targeted marketing strategies.

📂 Repository Structure
Banking.ipynb: Python notebook for data cleaning and SQLAlchemy database loading.

bank.sql: SQL scripts for financial aggregation and risk segmentation.

Banking Dashboard.pbix: Standalone Power BI report file with all data and DAX measures included.
