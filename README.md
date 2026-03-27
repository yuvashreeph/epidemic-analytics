# 🚀 Epidemic Spread Analytics Dashboard

Real-time epidemic modeling using **Kafka, Spark, Neo4j, Flask, and Docker**.

---

## 📌 Overview

This project builds a **real-time big data pipeline** to simulate and analyze disease spread using contact tracing data.

It identifies:

* Super-spreaders
* Hotspot locations
* Safe zones

---

## 🏗️ Architecture

```
Kafka → Spark Streaming → ETL → Spark Analytics → Neo4j
                                      ↓
                     Neo4j Bloom + Flask (Plotly Dashboard)
                                      ↓
                                 Docker
```

---

## ⚙️ Tech Stack

* Kafka (Streaming)
* PySpark (Processing + Analytics)
* Neo4j (Graph Database)
* Flask (Web App)
* Plotly (Visualization)
* Docker (Deployment)

---

## 🚀 How to Run

```bash
# Start Kafka
zookeeper-server-start.sh config/zookeeper.properties
kafka-server-start.sh config/server.properties

# Run Producer
python producer.py

# Run Spark
python spark_stream.py

# Run Dashboard
python app.py
```

Open: http://127.0.0.1:5000

---

## 🐳 Docker

```bash
docker build -t epidemic-dashboard .
docker run -p 5000:5000 epidemic-dashboard
```

---

## 🔥 Features

* Real-time data streaming
* Graph-based contact modeling
* Spark analytics (degree, hotspots)
* Interactive dashboard with maps

---

## 👩‍💻 Team

* Shinigdapriya Sathish
* Yuvashree P H

---

## 📜 Note

Academic project for Big Data Management Lab.
