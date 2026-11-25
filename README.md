# Hadoop Ecosystem

**Data Engineering 1 · SRH Hochschule Heidelberg**  
Sumit Kulhadia

---

## Contents

| File | Description |
|---|---|
| `Hadoop_Ecosystem.html` | Interactive lecture guide — Architecture diagrams, HDFS, YARN, MapReduce vs Spark, Data Lake vs DWH, and hands-on lab |

---

## Getting Started

```bash
# 1. Clone this repository
git clone https://github.com/srh-data-engineering/hadoop-ecosystem.git

# 2. Open the guide in your browser
open Hadoop_Ecosystem.html        # macOS
xdg-open Hadoop_Ecosystem.html   # Linux
```

No setup script needed — the HTML is a self-contained lecture guide.

---

## Hands-On Lab

The lab deploys a local Hadoop cluster (NameNode, DataNode, ResourceManager, NodeManager, History Server) using Docker Compose.

All required files are in the **spark-cluster** folder of the course repository:  
[github.com/binhvd/Data-Engineer-1](https://github.com/binhvd/Data-Engineer-1)

```bash
# Clone the course repo and navigate to the cluster folder
git clone https://github.com/binhvd/Data-Engineer-1
cd Data-Engineer-1/spark-cluster

# Start the cluster
sudo docker-compose up -d

# Access HDFS UI after ~2 minutes
# Open browser: http://[Ubuntu IP]:9870

# Stop and clean up
sudo docker-compose down -v
```

> **Requirement:** Ubuntu 22.04 VM with Docker installed.

---

## Topics Covered

| Section | Key Concepts |
|---|---|
| Foundations | Hadoop, HDFS, YARN, MapReduce, Spark |
| Architecture | NameNode, DataNode, ResourceManager, NodeManager |
| HDFS | Block storage, replication, rack awareness, read/write paths |
| YARN | Job scheduling, container lifecycle, ApplicationMaster |
| Data Processing | MapReduce vs Spark — latency, fault tolerance, use cases |
| Slide 16 | Hadoop ecosystem map — Hive, Pig, HBase, Kafka, Sqoop |
| Slide 17 | Enterprise Data Lake architecture |
| Data Lake vs DWH | Schema-on-read vs schema-on-write, use cases, tools |
