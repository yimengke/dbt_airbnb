# 🏡 Airbnb Analytics Project with dbt

This project analyzes Airbnb listings, hosts, and reviews using a modern data stack with **dbt** for transformation and **Preset (Superset)** for visualization.

This project models and analyzes Airbnb data using dbt. The pipeline transforms raw data into a structured data warehouse through multiple layers including staging, dimensional modeling, and reporting. The final data is visualized in an executive dashboard built with Preset (Apache Superset). The diagram below illustrates the full data lineage from raw sources to dashboards:
![Lineage Graph](https://github.com/yimengke/dbt_airbnb/raw/main/dbtlearn/assets/lineage_graph.png)



## 🔧 Project Structure

- **models/**  
  dbt models for staging, transformation, and mart layers

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
