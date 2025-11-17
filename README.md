# Electric-Vehicle-Growth-Analytics-for-Sustainable-Transport

This project demonstrates a big data analytics pipeline for analyzing Electric Vehicle (EV) adoption, energy use, and charging infrastructure using Google Cloud Platform (GCP), Snowflake, Python, SQL, and Power BI, aligned with SDG 7 & 13 (Affordable & Clean Energy, Climate Action).

![gsc_snw](https://github.com/user-attachments/assets/99e24532-15fa-4659-a6ed-3801f3254f11)

# Project Workflow
1. Data Ingestion (Raw Dataset → GCS)

Raw CSV datasets were uploaded from local storage to Google Cloud Storage (GCS) using Python scripts via Google Cloud Console.

User-friendly visual interface used to create buckets and transfer files securely.

2. Data Storage

Data stored in GCS under g8_2nd_bucket in the bigdataG8 project.

Provides a central, scalable, and durable repository for efficient retrieval and integration with platforms like Snowflake or BigQuery.

3. Data Ingestion (GCS → Snowflake)

Auto-ingestion setup using Pub/Sub and Snowpipe for real-time data loading.

Snowpipe detects new files in GCS and ingests them into Snowflake automatically, ensuring data consistency and seamless analytics workflow.

4. Data Transformation

Performed SQL transformations in Snowflake:

Cleaning and handling missing values

Restructuring and aggregations

Creating snapshot tables for historical data and production tables for latest data

Snowflake’s scalability enabled efficient processing of large datasets.

5. Data Analytics

Exploratory Data Analysis (EDA) conducted using Snowflake Notebook with Python & SQL.

Removed irrelevant columns (DOL_VEHICLE_ID, LEGISLATIVE_DISTRICT) and standardized data types (e.g., POSTAL_CODE → INT) for consistency.

6. Data Visualization

Processed data visualized in Power BI for interactive dashboards and insightful visualizations.

Facilitates decision-making and monitoring EV adoption trends effectively.

# Tools & Technologies

Cloud & Data Storage: Google Cloud Storage, Snowflake

Data Pipeline & ETL: Python, Snowpipe, Pub/Sub

Data Analysis: SQL, Python

Data Visualization: Power BI

# Project Highlights

End-to-end big data pipeline from ingestion to visualization

Real-time data ingestion with Snowpipe & Pub/Sub

Cleaned and structured EV population data for analytics

Interactive dashboards supporting sustainable transport and SDG goals


