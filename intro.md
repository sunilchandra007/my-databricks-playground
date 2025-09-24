# 🚀 Introduction to Databricks

- A data platform, built on **Apache Spark**
- combines all three into a single platform
   - **data engineering** - Data ingestion pipeline, job, ETL
   - **data science** - analytics
   - **machine learning** - workflows 

---

## 🚀 Apache Spark
Apache Spark is an open-source **distributed computing** system designed for big data processing. 

**Key Features:**
- Fast in-memory data processing
- Supports SQL and machine learning
- Scales across clusters
- Ideal for ETL, analytics, and data science
- Supports batch and streaming workloads

## 💾 Delta Lake
Delta Lake is a **storage layer** built on top of Apache Spark. It is backbone of Databricks’ **Lakehouse** architecture.

**Key Features:**
- ACID transactions for data consistency
- Schema evolution and enforcement
- Time travel (query historical versions of data)
- Data linege and Audit
- Unified Batch and streaming workloads



## MLflow

An open-source platform for managing the entire machine learning lifecycle. Fom tracking experiments to managing model deployment, it simplifies the process of building and operationalizing ML models.

---

## 💼 Common Use Cases

- 📊 Real-Time Data Processing and Big Data Analytics and 
- 🧠 Machine Learning - Train and deploy ML models with built-in tools and framework - MLflow, TensorFlow,
- 🔄 Data Engineering - Data ingestion and transformation, Data Pipelines, ETL, Jobs
- 📉 Data Governance - Role-based access control, **Unity Catalog**, and compliance support
- 🕒 Unified Workspace: Combines notebooks, dashboards, jobs, and collaboration tools.

---

## 🛠️ Getting Started

1. 🔧 Create a Databricks workspace.
2. 📓 Launch a notebook.
3. 🔗 Connect to data sources (e.g., Delta Lake, external databases).
4. 💻 Start coding in **Python**, **SQL**, **Scala**, or **R**.

   - Workspace - logically holds the notebooks, that could also have folders
   - Catalog - logically holds tables and volumes
     - catalog.schema.table
     - catalog.schema.volume


Free edition provides 
- Serverless PySpark - all purpose
- SQL Warehouse

---

## 📚 Learn More

Explore the official documentation:  
👉 Databricks Videos
👉 [Delta Lake](https://www.youtube.com/watch?v=HQvAl0Bwpu8)

---

