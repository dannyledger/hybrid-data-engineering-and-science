## 🔁 Module 2: Pipelines & Orchestration

### 🧠 Overview
This module focuses on automating the movement and transformation of data through pipelines. You'll learn the core principles of ETL/ELT, how to build reliable workflows using tools like Airflow or Prefect, and how to test and monitor these systems.

### 📚 References
- *Designing Machine Learning Systems* — Chip Huyen (Pipelines and production systems)
- *Fundamentals of Data Engineering* — Joe Reis & Matt Housley (Ch. 3–5 on pipeline design, orchestration, and testing)
- Airflow documentation: https://airflow.apache.org/
- Prefect docs: https://docs.prefect.io/
- Real Python ETL examples: https://realpython.com/etl-pipeline-python/

### 🧪 Tasks & Exercises
- [ ] Design a basic ETL flow in pseudocode (Extract → Transform → Load)
- [ ] Write an ETL function in Python that loads, processes, and saves a file
- [ ] Create a simple Airflow DAG with 2–3 dependent tasks
- [ ] Test transformation functions using pytest
- [ ] Add logging to a Python script with timestamps and status info

### 📄 Project
**Title:** Scheduled ETL DAG to Process and Upload Data
**Deliverables:**
- `airflow_etl_dag.py`
- `tests/` with at least one test script
- Logs demonstrating job execution
- Documentation in `README.md`

### 📝 Progress Log (`notes.md`)
Use this to track:
- DAG concepts and how scheduling works
- Pain points with Airflow or Prefect setup
- Which pipeline architecture concepts made sense
- Insights from testing/logging experiments
