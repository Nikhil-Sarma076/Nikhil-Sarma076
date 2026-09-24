<!-- Banner -->
<h1 align="center">Hi, I'm Nikhil Sarma 👋</h1>

<p align="center">
  <b>Data Platform Engineer</b> · Lakehouse Systems · Distributed Data Infrastructure
</p>

<p align="center">
  <a href="https://github.com/Nikhil-Sarma076">
    <img src="https://img.shields.io/badge/Focus-Apache_Iceberg_%2B_Delta_Lake-00ADD8?style=for-the-badge&logo=apache&logoColor=white" alt="Focus"/>
  </a>
  <img src="https://img.shields.io/badge/Zero--JVM-Python_Native-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Zero JVM"/>
  <img src="https://img.shields.io/badge/Cloud-AWS_EMR_on_EKS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS"/>
</p>

<p align="center">
  📍 Vijayawada, India &nbsp;·&nbsp; 🟢 Open to data engineering roles
</p>

---

### 🚀 What I do

I build the shared **data infrastructure** that product teams stand on — reusable
libraries, distributed execution engines, and real production IaC. Most at home in
the messy middle where **Apache Iceberg / Delta Lake**, distributed compute, and
self-service tooling meet. I like tools that are **cheaper, faster, and honest
about their own data quality**.

---

### 🏗️ What I work on at Infor (DataFabric / Lakehouse Platform)

- 🧱 Built the **shared lakehouse layer for 4 product lines** — self-service Iceberg tables + SQL access, one platform
  instead of per-product duplication.
- ⚡ Designed an **async execution engine** decoupling API traffic from EMR's
  ~1 req/sec limit via **SQS FIFO** — absorbing ~200 concurrent requests, ~180
  jobs/hour, per-tenant ordering + dead-letter isolation.
- 📉 Drove a **3-stage performance evolution** on batch ingestion (in-pod → EMR-on-EKS
  → tuned Spark) cutting **1B-row runtime from ~48h to 5h43m (~8.5×)**.
- 🧰 Shipped a **40+ module shared Python library** (Spark sessions, Iceberg
  lifecycle, 3-format ingestion, stateless EMR client, reconciliation) — cutting
  per-service integration code ~70%.
- 🏗️ Provisioned **8 Terraform modules** across 3 envs: EMR Virtual Clusters,
  SQS FIFO, DocumentDB, S3, IAM — with a self-managed **Iceberg REST catalog**
  (Lakekeeper) and **AWS Glue Catalog** selected per consumer.

---

### 🧊 Open-source projects — a local-first, dual-format lakehouse toolkit

> One theme: **run a real lakehouse on your laptop, in either format, with no JVM
> and no cloud account.** `docker compose up` and go.

<table>
  <tr>
    <td width="50%" valign="top">

#### 🔨 [lakehouse-forge](https://github.com/Nikhil-Sarma076/lakehouse-forge)
**Dual-format ingestion toolkit**

Convert CSV / JSON / Parquet into **Apache Iceberg _or_ Delta Lake** — you pick
the format per request. FastAPI + MinIO + Trino, zero-JVM (PyIceberg + delta-rs).
Async job queue, partition transforms, schema evolution, native Delta `MERGE`.

`FastAPI` · `PyIceberg` · `delta-rs` · `MinIO` · `Trino` · `React`

  </td>
    <td width="50%" valign="top">

#### 🔍 [lakehouse-checker](https://github.com/Nikhil-Sarma076/lakehouse-checker)
**Dual-format data-quality CLI**

Detects schema drift, null spikes, duplicate PKs, and row-count drops on **Delta
_and_ Iceberg** tables. **O(1)** metadata reads + **O(Δ)** scans of only new-commit
files — zero full-table scans, zero Spark, zero JRE. Runs as a tiny K8s CronJob.

`delta-rs` · `PyIceberg` · `PyArrow` · `Terraform` · `Kubernetes`

  </td>
  </tr>
</table>

---

### 🧠 Tech stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

![Apache Iceberg](https://img.shields.io/badge/Apache_Iceberg-1E90FF?style=flat-square&logo=apache&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-00ADD8?style=flat-square)
![Trino](https://img.shields.io/badge/Trino-DD00A1?style=flat-square&logo=trino&logoColor=white)
![Apache Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PyArrow](https://img.shields.io/badge/PyArrow-FF7F0E?style=flat-square)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![EMR on EKS](https://img.shields.io/badge/EMR_on_EKS-FF9900?style=flat-square&logo=amazoneks&logoColor=white)
![S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![Glue](https://img.shields.io/badge/Glue_Catalog-8C4FFF?style=flat-square&logo=amazonaws&logoColor=white)

![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

**Patterns:** CDC · SCD Type 2 · Multi-Tenancy · Event-Driven Architecture ·
Rate-Limit Decoupling · Reconciliation

---

<p align="center"><i>Building tools that make pipelines cheaper, faster, and honest about their quality.</i></p>
