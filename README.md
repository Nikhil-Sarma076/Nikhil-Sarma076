
### Hi, I'm Nikhil Sarma 👋

Data engineer focused on **lakehouse architecture** — Apache Iceberg, Delta Lake, PySpark, and data reliability. Building tools that make pipelines cheaper, faster, and honest about their quality.

---

**What I work on at Infor**

- Built a pip-installable file-to-Iceberg migration tool (CSV/JSON/NDJSON/Parquet → Iceberg via Glue Catalog + S3 Tables) deployed on EMR-on-EKS — reduced warehouse costs across 4 products
- Implemented Trino query engine with streaming support for the Ontology model-training pipeline
- Dual catalog backend (Nessie REST / AWS S3 Tables) switchable via session-factory API; infra via Terraform + Kubernetes

---

**Open source projects**

| Project | What it does |
|---|---|
| [deltacheck]([https://github.com/YOUR_USERNAME/deltacheck](https://github.com/Nikhil-Sarma076/deltacheck)) | Delta Lake data quality CLI — detects schema drift, null spikes, duplicate PKs by reading the transaction log. O(1) metadata reads, O(Δ) file scans. Zero full-table Spark scans. |
| [iceberg-ingestion-toolkit]([https://github.com/YOUR_USERNAME/iceberg-ingestion-toolkit](https://github.com/Nikhil-Sarma076/Iceberg-Forge-Local-Lakehouse-Stack)) | Python-native REST service (FastAPI + PyIceberg + MinIO + Trino) that converts CSV/JSON/Parquet into Iceberg tables. Async job queue, partition transforms, schema evolution. No Spark. |

---

**Stack**

`Apache Iceberg` `Delta Lake` `PySpark` `Trino` `Apache Airflow`  
`AWS (EMR · S3 · Glue · EKS)` `Kubernetes` `Terraform` `FastAPI` `Python` `SQL`

---

**Currently building:** `lakehouse-sync` — incremental CDC from Postgres into Iceberg using Airflow

📍 Vijayawada, India · Open to data engineering roles
      
