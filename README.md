# 📊 End-to-End Data Pipeline & Sentiment Analysis on Bing News with Microsoft Fabric  

## 🚀 Project Overview  
This project demonstrates a complete **data engineering pipeline** built using **Microsoft Fabric**.  
It showcases how raw **Bing News data** can be ingested, transformed, analyzed, and visualized into **actionable insights** through an automated workflow.  

## 📌 Problem Statement  
In today’s digital era, organizations are overwhelmed with massive volumes of **unstructured news data** generated every second. Without automation, this creates several challenges:  

- ⏳ **Delayed Decision-Making**: Raw data is scattered and unprocessed, slowing down business-critical insights.  
- 📉 **Company Reputation Risks**: Negative news or public sentiment may go unnoticed, impacting brand image.  
- 🤝 **Loss of Public Trust**: Organizations fail to respond quickly to sentiment shifts.  
- 🔄 **Inefficient Data Handling**: Manual data collection, lack of incremental updates, and fragmented tools waste resources.  

These challenges directly affect business decision-making, market competitiveness, and stakeholder trust.  

## 🎯 Project Objective  
This project provides a complete end-to-end solution using **Microsoft Fabric** to overcome the above challenges by:  

- **Resource Setup 🏗️** – Provisioning **Azure Resource Group**, Fabric **capacity**, and a dedicated **workspace**.  
- **Automated Data Ingestion 📥** – Integrating **Bing News REST API** into pipelines and storing results in a **Lakehouse** (JSON, Tables, CSVs).  
- **Data Transformation 🔧** – Cleaning, structuring, and implementing **incremental load mechanisms** via notebooks.  
- **Sentiment Analysis 🧠** – Applying **NLP techniques** to classify news as **Positive, Negative, or Neutral**, enabling organizations to track public opinion.  
- **Pipeline Orchestration 🔄** – Automating workflows by connecting multiple notebooks in **pipelines** with scheduling for real-time or batch updates.  
- **Business Insights 📊** – Delivering **decision-ready insights** through an interactive **Power BI dashboard** (trends, keyword analysis, regional sentiment).  

## ✅ Outcome  
A **scalable, automated system** that transforms raw unstructured news data into actionable insights, helping organizations:  

- Make faster **data-driven decisions**  
- Protect **company reputation**  
- Maintain **public trust**  


---

## 🏗️ Architecture Workflow  

### 1️⃣ Fabric Setup  
- Created **Resource Group**  
- Assigned **Fabric Capacity (License)**  
- Created **Fabric Workspace** and attached it to capacity  

### 2️⃣ Data Ingestion (Pipeline)  
- Built a pipeline using **Copy Data activity**  
- **Source**: REST API
- https://www.searchapi.io/api/v1/search
- ?api_key=V4QbmTZ5uUYUGZWyea5VSF8T&engine=bing_news&location=10003%2CNew+York%2CUnited+States&q=latest+news&num=1000

- - **Destination**: Data Lakehouse → JSON files  

### 3️⃣ Data Transformation (Notebooks)  
- **Notebook 1: Raw → Structured → Tables**  
- Data cleaning & structuring  
- Stored into **Lakehouse Tables**  
- Implemented **Incremental Load**  

- **Notebook 2: Sentiment Analysis**  
- Applied **sentiment scoring** on selected columns  
- Stored results back into **Lakehouse**  

### 4️⃣ Pipeline Orchestration  
- Combined multiple notebooks into a **single pipeline container**  
- Orchestrated **end-to-end workflow** (ETL + Analysis)  
- Configured **scheduling (timer triggers)**  
- Example: In enterprise cases, pipelines can auto-refresh whenever **new data arrives**  

### 5️⃣ Visualization (Dashboard)  
- Built an **interactive Power BI dashboard** (attached `.pbix` file)  
- **Insights include:**  
- 😀 Positive / 😡 Negative / 😐 Neutral sentiment trends  
- 🔑 Keyword-based sentiment  
- 🌍 Regional sentiment insights  

---

## 📂 Repository Contents  
- `notebooks/` → Transformation & Sentiment Analysis notebooks  
- `pipelines/` → End-to-End orchestration pipelines  
- `dashboard/` → Power BI `.pbix` file  
- `lakehouse/` → Processed & structured data (JSON, Tables, CSVs)  

---

## ⚡ Features  
- End-to-end **automated pipeline**  
- Handles **raw → structured → analytical** data lifecycle  
- Real-time **sentiment analysis**  
- Supports **incremental data loading**  
- **Enterprise-ready** scheduling & orchestration  
- Interactive **Power BI dashboard**  

---

## 🛠️ Tech Stack  
- **Microsoft Fabric** (Capacity, Workspace, Lakehouse)  
- **Data Engineering Pipeline** (Copy Data, Orchestration)  
- **Notebooks** (PySpark / Python)  
- **Sentiment Analysis** (Text/NLP methods)  
- **Power BI** for visualization  

---

## ▶️ How to Run  

- Clone the repository  
 ```bash
 git clone https://github.com/<your-username>/<your-repo>.git
- Import the notebooks into Microsoft Fabric Workspace
- Configure pipeline with:

Source: REST API
Destination: Lakehouse

- Run the Data Ingestion pipeline
- Execute Notebooks:

Transformation Notebook
Sentiment Analysis Notebook

- Open the Power BI dashboard (.pbix)
Connect to Lakehouse tables
- (Optional) Set up scheduled refresh for automation.

-------









  
