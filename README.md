# 🏡 Airbnb Analytics Project with dbt

This project analyzes Airbnb listings, hosts, and reviews using a modern data stack with **dbt** for transformation, **Snowflake** as the data warehouse, and **Preset (Superset)** for visualization.

The pipeline transforms raw Airbnb data into a structured analytics layer through dbt models — including staging, dimensional modeling, and reporting. These models are built and stored in **Snowflake**, ensuring scalable and performant data processing. The final insights are presented in an executive dashboard built with **Preset (Apache Superset)**.
 The diagram below illustrates the full data lineage from raw sources to dashboards:
![Lineage Graph](https://github.com/yimengke/dbt_airbnb/raw/main/dbtlearn/assets/lineage_graph.png)

## 🔧 Imput Data Entity Relationship Diagram

Below is the overview of the input data for my project.
![Lineage Graph](https://github.com/yimengke/dbt_airbnb/raw/main/dbtlearn/assets/ERD.jpg)



## 🔧 Project Structure

- **models/**  
  dbt models for staging layer, dimensional data warehouse layer, and report layers with merged tables
  
- **seeds/**  
  Seed data (e.g., full moon calendar)

- **snapshots/**  
  SCD Type 2 snapshots to track data changes

- **analyses/**  
  ad-hoc SQL analyses for exploration

- **macros/**  
  Custom Jinja macros for reuse in dbt models

- **tests/**  
  Generic and singular tests for data quality

## 📊 Dashboard Overview

🔗 [Click here to explore the interactive dashboard](https://040c4d1e.us2a.app.preset.io/superset/dashboard/p/qbkBWBbWpPV/)

![Dashboard Demo](dbtlearn/assets/dashboard.gif)

The dashboard is organized into three sections:

### 1. Hosts
- Total number of hosts
- Growth trend of new hosts (MoM)

### 2. Listings
- New listings over time
- Price distribution by room type
- Superhost distribution

### 3. Reviews
- Sentiment trend over time
- Sentiment comparison on full moon vs non-full moon days

## 🚀 How to Run Locally

1. Clone this repo  
```bash
git clone https://github.com/yimengke/dbt_airbnb.git
