# Cyprien Kelma — Data Engineer

Final-year software engineering student at ISEN Lille, currently in a Data Engineer apprenticeship at Decathlon Digital.
Building production-grade data platforms on GCP, AWS and Databricks.
Available for a permanent contract from September 2026.

---

## Main Projects

### 1. DroneFleet Optimizer — Real-Time Fleet Management Infrastructure

[Full Website Documentation](https://cyprienkelma.github.io/dronefleet-optimizer/en/) 

A complete event-driven system for coordinating emergency medical delivery drone fleets in real time.

- Architected a polyglot microservices system (Python FastAPI, Java Spring Boot) with Pub/Sub messaging, achieving sub-500ms latency for critical delivery operations
- Designed and solved a Vehicle Routing Problem with Pickup and Delivery (VRPPD) using Google OR-Tools, with an optimistic concurrency model to handle concurrent optimization cycles safely
- Deployed fully on GCP using Terraform (Cloud Run, Firestore, Artifact Registry), with a local dev environment via Docker Compose and emulators — zero cloud cost during development
- Built an ELT analytics pipeline (dbt, BigQuery) to process drone telemetry and expose a real-time monitoring dashboard with Streamlit

**Stack:** Python, Java, GCP, Terraform, Pub/Sub, Firestore, dbt, BigQuery, Docker, GitHub Actions

[Repository](https://github.com/CyprienKelma/dronefleet-optimizer)

---

### 2. Cloud ELT Platform — Reusable Data Infrastructure Template

A production-ready ELT pipeline template deployable on any GCP account in under 20 minutes. Built as part of a Cloud Computing course (M2), graded 18/20.

- Provisioned the full infrastructure with Terraform (IaC): GCS buckets for dev and prod, BigQuery datasets with lifecycle policies, IAM service accounts following least-privilege principles
- Orchestrated daily ingestion and transformation workflows with Prefect Cloud, with retry logic and support for both local and cloud execution modes
- Modelled data in BigQuery using dbt with a full medallion architecture (staging, intermediate, marts) and a star schema exposed to Power BI
- Set up CI/CD with GitHub Actions to automatically regenerate and publish the dbt documentation site on every production merge

**Stack:** GCP (GCS, BigQuery, Cloud Run), Terraform, Prefect Cloud, dbt, Python, GitHub Actions, Power BI

[Repository](https://github.com/Summers-Team/school-m2-bi-project)

---

### 3. Distributed Data Architecture — Scalable Backend System

A distributed, multi-modal storage architecture built to handle TB-scale data volumes, developed as a fourth-year engineering project.

- Designed horizontal scaling with Kubernetes (K3s) and Helm across PostgreSQL (relational), Cassandra (high-write NoSQL), Neo4j (graph), and Redis/KeyDB (cache)
- Built a daily ELT pipeline orchestrated by Airflow on Kubernetes: Bronze (raw extraction) → Silver (Parquet, cleaning) → Gold (DuckDB analytical warehouse)
- Developed the backend API in NestJS with multi-storage integrations and MinIO as an S3-compatible data lake

**Stack:** Kubernetes, Spark, Airflow, PostgreSQL, Cassandra, Neo4j, Redis, MinIO, DuckDB, NestJS

[Repository](https://github.com/CyprienKelma/Projet-M1) - [Concept Paper (French)](https://drive.google.com/file/d/1x0aIjapqhaVRPJEvIRTzORIR9aschmZv/view?usp=sharing)

---

## Experience

**Data Engineer, Apprenticeship** — Decathlon Digital, Lille (Sep 2025 – End of Aug 2026)

- Built a self-service analytics platform backed by Databricks, Cloud Run and BigQuery, enabling data analysts to ship production-grade data apps, reducing delivery time from days to hours through AI-assisted development workflows

- Drove self-service data adoption by building core dbt models and mentoring analysts on software engineering best practices (Git workflows, CI/CD, automated testing), while industrializing an ML forecasting pipeline with MLFlow and Airflow orchestration serving 10+ sports business analysts and financial team members

- Optimized production pipelines performances by implementing Auto-Compact, Partitioning, Idempotency, Vacuum and incremental logic on Delta tables format, reducing execution time by 40% and improving downstream read efficiency

**Data Engineer, Internship** — Decathlon Belgium, Brussels (May 2025 – Aug 2025)

- Built and deployed a production-grade ETL pipeline on Databricks processing high-volume logistics data from a REST API into BigQuery, ensuring data integrity with Great Expectations and Pydantic across thousands of daily deliveries.

- Led a reporting pipeline on AWS using Airflow (MWAA) to orchestrate Docker containers on Kubernetes (EKS), automatically generating 100+ slide weekly BI reports and eliminating hours of manual work.

- Maintained and improved PySpark transformation codebase across 5+ Databricks jobs, developed and refactored dbt models, resolved critical Airflow DAG bugs, and contributed a fix to an open-source library within a CI/CD workflow

---

## Stack

- **Data Engineering:** PySpark, Databricks, Delta Lake, dbt, Airflow, Prefect, ETL/ELT, Great Expectations, Pydantic
- **Warehouses & Storage:** BigQuery, PostgreSQL, Snowflake, Cassandra, Redis, MongoDB
- **Cloud:** GCP (BigQuery, Cloud Run, Pub/Sub, GCS, Firestore), AWS (S3, EKS, MWAA, ECR)
- **Infrastructure:** Terraform, Docker, Kubernetes, GitHub Actions
- **Languages:** Python, SQL, Java (Spring Boot)

---

## Education

**Master of Computer Science** — ISEN Lille, French Engineering School (2021 – 2026)

> Data Structures & Algorithms, Java, Distributed Systems, Machine Learning, Deep Learning, DevOps, Cloud Computing, Database Management (SQL & NoSQL), Operations Research, Metaheuristics, Spark.

---

## Contact :
- LinkedIn : [cyprien-kelma](https://www.linkedin.com/in/cyprien-kelma/)
- Email : cyprien.kelma@gmail.com
