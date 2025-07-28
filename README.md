# 🏡 Airbnb Analytics Project with dbt

This project analyzes Airbnb listings, hosts, and reviews using a modern data stack with **dbt** for transformation and **Preset (Superset)** for visualization.

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
   git clone https://github.com/yourname/dbt_airbnb.git
