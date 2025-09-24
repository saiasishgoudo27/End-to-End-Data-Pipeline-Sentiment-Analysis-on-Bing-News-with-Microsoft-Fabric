# 📊 End-to-End Data Pipeline & Sentiment Analysis on Bing News with Microsoft Fabric  

## 🚀 Project Overview  
This project demonstrates a complete **data engineering pipeline** built using **Microsoft Fabric**.  
It showcases how raw **Bing News data** can be ingested, transformed, analyzed, and visualized into **actionable insights** through an automated workflow.  

---

## 🌟 Key Highlights  
- ⚡ Resource provisioning and Fabric capacity setup  
- 🌐 Data ingestion via REST API (Bing News)  
- 🔄 Data transformation and incremental load handling  
- 😀 Sentiment analysis on ingested news data  
- 🔗 Automated pipelines for orchestration  
- 📊 Interactive Power BI dashboard for insights  

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

## ScreenShots :

<img width="1919" height="819" alt="Screenshot 2025-09-24 232819" src="https://github.com/user-attachments/assets/4800fd74-aedd-4af1-9c92-cddabb0eaf68" />

<img width="1918" height="839" alt="Screenshot 2025-09-24 232854" src="https://github.com/user-attachments/assets/c179d5dc-405a-4cb1-bb58-177f6439fdfc" />

<img width="1913" height="906" alt="Screenshot 2025-09-24 232938" src="https://github.com/user-attachments/assets/ce82ac46-05d2-48fc-b45f-291556077f9e" />

<img width="1919" height="902" alt="Screenshot 2025-09-24 233221" src="https://github.com/user-attachments/assets/7be18716-0497-47ee-a839-b95cd393cd6d" />

<img width="1918" height="915" alt="Screenshot 2025-09-24 233304" src="https://github.com/user-attachments/assets/b186bab6-eed5-4718-b1c9-dfbaa942d8c7" />

<img width="1919" height="916" alt="Screenshot 2025-09-24 233327" src="https://github.com/user-attachments/assets/e290a928-3a4c-48b5-a7c4-a35b095eaac0" />

<img width="1919" height="1014" alt="Screenshot 2025-09-22 150329" src="https://github.com/user-attachments/assets/94534391-b314-4c5c-adc7-7108c79d4949" />

-------
## Dashboard:

<img width="1328" height="739" alt="Screenshot 2025-09-22 155949" src="https://github.com/user-attachments/assets/7030cd57-9c84-4654-b729-c93b07a678e4" />









  
