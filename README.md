# Laptop-Specs-Analytics-End-to-End-Data-Engineering-Project

![Domain](https://img.shields.io/badge/Domain-Consumer%20Electronics-blue?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-Python|PostgreSQL|Tableau-green?style=for-the-badge)
![Project Type](https://img.shields.io/badge/Type-Data%20Engineering%20%26%20Visualization-yellow?style=for-the-badge)

## Python------>SQL------>Tableau

## Overview

This end-to-end data engineering and analytics project focuses on analyzing synthetic laptop features data. It begins with automated data retrieval from Kaggle, followed by preprocessing, feature engineering, and transformation in Python. The cleaned data is pushed into a PostgreSQL database and visualized through an interactive Tableau dashboard to derive brand-wise and specification-based insights to help a customer make choices for buying a laptop from the market.

## Objectives

- Automate data ingestion using the Kaggle API.
- Clean and engineer laptop features (CPU type, screen, storage) using Python.
- Store structured data in a PostgreSQL database.
- Visualize trends and comparisons using Tableau dashboards.

## Tools & Technologies

- **Data Collection**: Kaggle API  
- **Processing**: Python (pandas, numpy, seaborn, matplotlib)  
- **Database**: PostgreSQL  
- **Visualization**: Tableau  

## Key Steps

### 1. Data Ingestion

- Downloaded the laptop price dataset from Kaggle using the Kaggle API.
- Loaded the Excel file into a Pandas DataFrame.

### 2. Data Cleaning & Feature Engineering

- Removed duplicates and null values.
- Parsed complex columns (e.g., ScreenResolution) to extract features like `Touchscreen`, `IPS`, `PPI`, etc.
- Standardized units (e.g., RAM to integer, Weight to float).
- Created flags for types of storage: SSD, HDD, Flash, Hybrid.
- Categorical transformation of CPU, GPU, and OS types.

### 3. Database Storage

- Created a PostgreSQL schema.
- Used SQLAlchemy to insert the transformed DataFrame into a table.
- Ensured column types were correctly mapped to SQL equivalents.

### 4. Data Visualization

- Connected Tableau to the PostgreSQL database.
- Built an interactive dashboard comparing:
  - Price distribution by brand, type, and specs.
  - Influence of touchscreen, IPS, storage types, and RAM.
  - GPU and OS preferences across companies.
  - Average prices by processor families.

## Highlights

- Clear data pipeline from **API to Dashboard**.
- **Modular and reusable** Jupyter Notebook for transformation logic.
- Dashboard enables **dynamic filtering** by brand, specs, and component types.
- Valuable business insights like:
  - **Touchscreen & IPS displays** increase price significantly.
  - **Intel Core i7 + SSDs** dominate the high-end market.
  - **Dell and Lenovo notebooks** are common in mid-tier pricing.

## Output

 **Dashboard Title**: *Laptop Insights Dashboard: Compare Brands, Features & Prices*  
[View Dashboard on Tableau](https://public.tableau.com/app/profile/anushree.biswas/viz/Compare_brands_price_features_for_laptops/Dashboard1)


