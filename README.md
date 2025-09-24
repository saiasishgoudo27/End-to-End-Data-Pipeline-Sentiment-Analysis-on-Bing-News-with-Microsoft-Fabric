📊 End-to-End Data Pipeline & Sentiment Analysis on Bing News with Microsoft Fabric
🚀 Project Overview

This project demonstrates a complete data engineering pipeline built using Microsoft Fabric. It showcases how raw Bing News data can be ingested, transformed, analyzed, and visualized into actionable insights through an automated workflow.

🌟 Key Highlights

⚡ Resource provisioning and Fabric capacity setup

🌐 Data ingestion via REST API (Bing News)

🔄 Data transformation and incremental load handling

😀 Sentiment analysis on ingested news data

🔗 Automated pipelines for orchestration

📊 Interactive Power BI dashboard for insights

🏗️ Architecture Workflow
1️⃣ Fabric Setup

🏢 Created Resource Group

📌 Assigned Fabric Capacity (License)

🗂️ Created Fabric Workspace and attached it to capacity

2️⃣ Data Ingestion (Pipeline)

⚙️ Built a pipeline using Copy Data activity

Source: REST API

https://www.searchapi.io/api/v1/search
?api_key=V4QbmTZ5uUYUGZWyea5VSF8T&engine=bing_news&location=10003%2CNew+York%2CUnited+States&q=latest+news&num=1000


Destination: Data Lakehouse → JSON files

3️⃣ Data Transformation (Notebooks)

📒 Notebook 1: Raw → Structured → Tables

Data cleaning & structuring

Stored into Lakehouse Tables

Implemented Incremental Load for efficiency

📒 Notebook 2: Sentiment Analysis

Applied sentiment scoring on selected columns

Stored results back into Lakehouse

4️⃣ Pipeline Orchestration

🔄 Combined multiple notebooks into a single pipeline container

▶️ Orchestrated end-to-end workflow (ETL + Analysis)

⏱️ Configured scheduling (timer triggers)

Example: In enterprise use cases, when working with real-time streaming data, the pipeline can be scheduled to refresh automatically whenever new data arrives.

5️⃣ Visualization (Dashboard)

📊 Built an interactive Power BI dashboard (attached .pbix file)

Insights include:

😀 Positive / 😡 Negative / 😐 Neutral trends

🔑 Keyword-based sentiment analysis

🌍 Regional sentiment insights

📂 Repository Contents

📁 notebooks/ → Transformation & Sentiment Analysis notebooks
📁 pipelines/ → End-to-End orchestration pipelines
📁 dashboard/ → Power BI .pbix file
📁 lakehouse/ → Processed & structured data (JSON, Tables, CSVs)

⚡ Features

✔ End-to-end automated pipeline
✔ Handles raw → structured → analytical data lifecycle
✔ Real-time sentiment analysis
✔ Supports incremental data loading
✔ Enterprise-ready scheduling & orchestration
✔ Interactive Power BI dashboard

🛠️ Tech Stack

🖥️ Microsoft Fabric (Capacity, Workspace, Lakehouse)

⚙️ Data Engineering Pipeline (Copy Data, Orchestration)

🐍 Notebooks (PySpark / Python)

🧠 Sentiment Analysis (Text processing, NLP methods)

📊 Power BI (Dashboarding)

▶️ How to Run

Clone the repository

git clone https://github.com/<your-username>/<your-repo>.git


Import notebooks into your Microsoft Fabric Workspace

Configure pipeline with:

REST API as Source

Lakehouse as Destination

Run the Data Ingestion Pipeline

Execute:

✅ Transformation Notebook

✅ Sentiment Analysis Notebook

Open the Power BI dashboard (.pbix) and connect it to your Lakehouse tables

(Optional) ⏱️ Set up scheduled refresh for automated updates

📸 Screenshots (Recommended to Add)

🖼️ Pipeline overview

🖼️ Notebook transformation process

🖼️ Power BI dashboard
