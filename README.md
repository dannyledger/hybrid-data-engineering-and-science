# 🚀 Hybrid Data Engineering + Data Science Learning Path

> **Goal:** This learning journey is self-directed and structured to explore various disciplines within data - from engineering to science. It is designed to build confidence, fluency, and hands-on capability through a practical, project-based approach without being tied to industry pressure or trends.

---

## 🧭 Learning Journey Structure (Non-Timebound)
| Module | Focus Area                          |
|--------|-------------------------------------|
| 1      | Data Engineering & Foundations      |
| 2      | Pipelines & Orchestration           |
| 3      | Analytics Engineering & Warehousing |
| 4      | Core Data Science & ML Principles   |
| 5      | Deployment, DevOps & Capstone       |

---

## 📁 Suggested GitHub Repo Structure
```
hybrid-data-engineering-datascience/
├── Module_1_Foundations/
│   ├── notes.md
│   ├── README.md
│   ├── exercises/
│   └── project/
│       ├── README.md
│       └── csv_to_parquet_to_s3.py
├── Module_2_Pipelines/
│   ├── README.md
│   ├── airflow_etl_dag.py
│   ├── tests/
│   └── logs/
├── Module_3_Analytics_Eng/
│   ├── README.md
│   ├── dbt_project/
│   └── bigquery_setup.md
├── Module_4_DataScience_ML/
│   ├── README.md
│   ├── core_concepts_notes.md
│   ├── from_scratch_implementations/
│   │   ├── linear_regression.py
│   │   ├── k_nearest_neighbors.py
│   │   └── decision_trees.py
│   └── ml_practice_notebooks/
├── Module_5_Deployment/
│   ├── README.md
│   ├── dockerfile
│   ├── deploy_instructions.md
│   └── README_project.md
├── capstone/
│   ├── risk_model_pipeline/
│   │   └── README.md
│   └── dashboard_project/
│       └── README.md
├── data/
│   ├── raw/
│   └── processed/
└── README.md
```

---

## 📦 Module 1: Data Engineering & Foundations
- SQL (joins, subqueries, window functions)
- Pandas (cleaning, grouping, reshaping)
- File formats: CSV, JSON, Parquet
- Data modelling: star & snowflake
- Cloud basics: AWS S3, IAM roles

**✅ Project:** Raw CSV → Cleaned Parquet → Upload to S3

---

## 🔁 Module 2: Pipelines & Orchestration
- ETL/ELT workflows
- Airflow / Prefect DAG setup
- Scheduling, dependencies
- Logging + pipeline testing with pytest

**✅ Project:** Airflow DAG with Python transformations + cloud integration

---

## 🧱 Module 3: Analytics Engineering & Warehousing
- dbt: cleaning and modelling layers
- BigQuery/Snowflake/Redshift basics
- Data warehouse optimisation (partitioning, indexing)
- Access control and cost management

**✅ Project:** Build an analytics-ready warehouse model using dbt

---

## 🤖 Module 4: Core Data Science & ML Principles
- *Data Science from Scratch* chapter-by-chapter builds
- Data exploration + preprocessing
- Implement linear regression, k-NN, Naive Bayes, trees from scratch
- Practice with scikit-learn for comparison
- Evaluation metrics and model validation

**✅ Project:** Rebuild 3 ML models from scratch + notebook comparisons

---

## ⚙️ Module 5: Deployment & Capstone
- Version control (GitHub best practices)
- Docker + environment setup
- Deployment basics (script vs model vs dashboard)
- Logging, error monitoring, retry logic
- Portfolio polish

**✅ Project:** Full ETL-to-ML pipeline or risk analysis dashboard, deployed and documented

---

## 🏁 Final Capstone Options
- **Risk Scoring System**
- **Data Quality Pipeline with Alerts**
- **Dashboard of Model Outputs from Clean Data Warehouse**

---

## 📚 Tools & Tech Stack
```
Languages: Python, SQL
Libraries: pandas, scikit-learn, pyarrow, boto3, dbt
Infra: PostgreSQL, BigQuery, S3, Docker
Workflow: Airflow, Prefect
Docs: dbt docs, MkDocs
Book References:
- *Data Science from Scratch* by Joel Grus
- *Designing Machine Learning Systems* by Chip Huyen
- *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* by Aurélien Géron
- *Effective Pandas* by Matt Harrison
- *Machine Learning with Python Cookbook* by Chris Albon
```
