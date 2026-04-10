# **UBER REAL-TIME DATA ENGINEERING PROJECT**

# 🚖 Real-Time Uber Data Engineering Pipeline

An end-to-end **real-time data engineering project** simulating an Uber ride-booking system using modern cloud and big data technologies.

---

## 📌 Project Overview

This project demonstrates how to build a **scalable real-time data platform** that ingests, processes, and analyzes ride-booking events.

It mimics how companies like Uber process continuous event streams to enable **real-time analytics and decision-making**.

---

## ⚡ Key Features

- 🔄 Real-time data ingestion using **Azure Event Hub (Kafka equivalent)**
- ⚙️ Stream processing with **Spark Structured Streaming**
- 🧱 **Medallion Architecture (Bronze → Silver → Gold)**
- 📊 Unified **One Big Table (OBT)** for analytics
- 🧠 **Metadata-driven pipelines** using Jinja
- 🔁 ETL pipelines using **Spark Declarative Pipelines (SDP)**
- 🏗️ Star Schema with **Slowly Changing Dimensions (SCD)**

---

## 🏗️ Architecture

![Architecture](architecture.png)

### 🔹 Flow:
1. User books ride via web app (FastAPI)
2. Event pushed to **Azure Event Hub**
3. Batch + mapping data ingested via **Azure Data Factory**
4. Data stored in **Bronze Layer (ADLS Gen2)**
5. Processed using **Spark Streaming (Silver Layer)**
6. Transformed into **Star Schema (Gold Layer)**

---

## 🧰 Tech Stack

| Layer        | Tools Used |
|-------------|-----------|
| Ingestion   | Event Hub, FastAPI |
| Orchestration | Azure Data Factory |
| Storage     | ADLS Gen2 |
| Processing  | PySpark, Spark Structured Streaming |
| Transformation | Spark Declarative Pipelines, Jinja |
| Modeling    | Star Schema, SCD |
| Platform    | Databricks |

---


## 📊 Data Pipeline Design

### 🔹 Bronze Layer
- Raw streaming + batch data
- Exact replica of source data

### 🔹 Silver Layer
- Cleaned + enriched data
- Streaming tables built using SDP

### 🔹 Gold Layer
- Business-level aggregations
- Fact & dimension tables

---

## 📈 Use Cases

- Real-time ride tracking analytics
- Demand pattern analysis
- Driver & customer behavior insights
- Operational dashboards

---

## 🧠 Key Learnings

- Building **real-time streaming pipelines**
- Handling **batch + streaming integration**
- Designing **metadata-driven ETL systems**
- Implementing **scalable data architectures**

---

## 🚀 How to Run

```bash
# Clone repo
git clone https://github.com/pritesh-sh21/Uber-Data-Engineering-Project

# Open in Databricks / Local environment
# Configure Azure resources (Event Hub, ADLS, ADF)

# Run pipelines step-by-step

)





