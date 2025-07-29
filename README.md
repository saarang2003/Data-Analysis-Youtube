# 📊 ETL Project: YouTube Data Analysis

## 📘 Introduction

This README document provides an overview of an **ETL (Extract, Transform, Load)** project developed to:

- Extract data from a YouTube channel using the **YouTube Data API** and **Python**
- Perform data transformations using the **Pandas** library
- Export the transformed data to a **CSV file**
- Load the data into a **MySQL** database (or optionally Snowflake)
- Create an interactive reporting dashboard using **Power BI**

---

## 🚀 Project Overview

This project demonstrates how to extract, transform, and visualize data from a YouTube channel using:

- **YouTube Data API**  
- **Python** for scripting and automation  
- **MySQL** for structured data storage  
- **Power BI** for visualization

It automates the end-to-end data pipeline to ensure the **Power BI dashboard stays up-to-date dynamically** with the latest YouTube statistics.

---

## 🛠 Tools Used

- **Python**: Scripting and orchestration
- **Pandas**: Data transformation and manipulation
- **YouTube Data API**: Fetching video/channel statistics
- **MySQL**: Structured local data storage
- **Snowflake** _(optional)_: Cloud-based data warehousing
- **Power BI**: Visualization and dashboard creation

---

## 📈 Dynamic Dashboard with Power BI

- Power BI is **connected directly to MySQL**
- Uses the **Power BI MySQL connector**
- **On-premises data gateway** configured for secure and live data refresh

---

## ⏱ Scheduled Automation

- Python script can be scheduled with **Windows Task Scheduler** (daily/hourly)
- **Power BI Service** is configured for **automatic refresh** from MySQL
- Ensures your dashboard always reflects the **latest YouTube data**

---

## 🔄 Project Steps

### ✅ Step 1: Data Extraction (YouTube API)
- Python + YouTube API are used to extract:
  - Video titles
  - Views
  - Likes
  - Published date
  - Video IDs, etc.

### ✅ Step 2: CSV File Creation
- Data is cleaned and transformed using **Pandas**
- Exported to a structured **CSV file**
- This acts as a staging/intermediate storage format

### ✅ Step 3: Load Data to MySQL (or Snowflake)
- CSV data is loaded into a **MySQL** table:
  - Uses **SQLAlchemy** and **pymysql** for DB connection
  - Handles duplicates with `ON DUPLICATE KEY UPDATE`

> Optional: Load into **Snowflake** for cloud-based scaling and BI integration

### ✅ Step 4: Reporting with Power BI
- Power BI connects to **MySQL** or **Snowflake**
- A dashboard visualizes:
  - Views/Likes trends
  - Publishing history
  - Top-performing videos
- Supports filtering, date slicing, and custom metrics

---

## 📊 Workflow Diagram

![Alt text](images/data_pipeline(1).png)


---

## 📺 The Dashboard

![Alt text](images/pie1.png)

- Real-time updates
- Video-level stats
- Channel growth trends
- Custom filters (date, views, likes, etc.)
