# End-to-End E-Commerce Analytics & Predictive Pipeline
## Project Overview

This project transforms over 1 million rows of raw transactional data into an interactive executive dashboard. By utilizing a hybrid stack of Python, SQL, and Power BI, the pipeline automates data governance, detects operational anomalies, and segments customers using Machine Learning to drive targeted business strategies.

### Dataset Information

•	Source: https://www.kaggle.com/datasets/kabilan45/online-retail-ii-dataset

•	Content: This dataset contains all transactions occurring between 01/12/2009 and 09/12/2011 for a UK-based and registered non-store online retail.

•	Scale: Over 1 million rows of transactional data including Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, and Country.

### Technical Workflow

  1. Data Governance & Cleaning (Python/Pandas)

    •	 Consolidated multi-year datasets and resolved critical data gaps, including the removal of 243k missing customer identifiers to ensure data integrity.

    •	Standardized schema naming conventions and converted temporal data into datetime objects for accurate time-series analysis.

  2. Digital Assurance & Anomaly Detection
   
    •	Engineered an automated outlier detection system using Z-Score statistical methods.

    •	Identified 1,180 transactional anomalies in order quantities, flagging potential wholesale errors or fraudulent activity before modelling.

  3. KPI Extraction (SQL / MySQL)
   
    •	Architected a relational database environment to monitor core business metrics.

    •	Developed complex SQL queries to calculate Monthly Revenue Growth and Customer Lifetime Value (CLV).

  4. Machine Learning for Segmentation (Scikit-Learn)
   
    •	Developed an RFM (Recency, Frequency, Monetary) model to quantify customer behaviour.

    •	Applied K-Means Clustering with StandardScaler to segment the customer base into distinct personas, such as "VIP/Top Spenders" and "At-Risk/Hibernating".

  5. Impactful Reporting (Power BI)
    
    •	Designed a multi-page executive dashboard featuring advanced analytics like 3-month sales forecasting and trend line analysis.

    •	Integrated multi-dimensional slicers (Geographic, Segment-based, and Temporal) to enable stakeholders to perform deep-dive root cause analysis.

### Key Insights

•	Segment Concentration: Identified that VIP customers (Cluster 0) contribute significantly higher average revenue per order ($469.98) compared to other segments.

•	Predictive Trends: Established a 95% confidence interval forecast for 2012 revenue trends based on historical seasonality.

•	Geographic Revenue Concentration: Identified that while the customer base is global, a significant majority of total revenue ($17.37M) is driven by specific top-performing countries, suggesting a need for localized marketing investment in underperforming regions.

•	Customer Retention Risk: Analysis revealed that over 99% of the customer base currently falls into the "At Risk / Hibernating" segment, highlighting a critical opportunity for a re-engagement campaign to stabilize long-term revenue.



<img width="1362" height="658" alt="image" src="https://github.com/user-attachments/assets/8a629d09-1f96-4d11-b298-2575f152c794" />


