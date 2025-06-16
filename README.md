# Hybrid Data Engineering + Data Science Learning Path
### Moving away from Datacamp's approach, and into something more unique to me.

--- 
> _**My prompt to GenAI:** Provide me with a learning journey which is self-directed and structured to explore various disciplines within data - from engineering to science. It should be designed to build my confidence, fluency, and hands-on capability through a practical, project-based approach without being tied to industry pressure or trends. Build off my existing understanding of Python and SQL, alongside referencing from text books I own._

---

## 🧭 Learning Journey Structure 
| Module | Focus Area                          |
|--------|-------------------------------------|
| 1      | Data Engineering & Foundations      |
| 2      | Pipelines & Orchestration           |
| 3      | Analytics Engineering & Warehousing |
| 4      | Core Data Science & ML Principles   |
| 5      | Deployment, DevOps & Capstone       |

---

## 📁 Initial Repo Structure
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


## 📦 Module 1: Data Engineering & Foundations

### 🧠 Overview
This module introduces core data handling and engineering concepts, including tabular data wrangling, SQL querying, file format optimisation, and early exposure to cloud tools. It sets the technical base for downstream analytics and ML work.

### 📚 References
- *Effective Pandas* — Matt Harrison (Chapters on cleaning, reshaping)
- *Data Science from Scratch* — Joel Grus (Data representation, stats intro)
- *Fundamentals of Data Engineering* — Joe Reis & Matt Housley (Ch. 1–2 on foundations and data lifecycle)
- Pandas docs: https://pandas.pydata.org/docs/
- AWS S3 documentation: https://docs.aws.amazon.com/s3/

### 🧪 Tasks & Exercises
- [ ] Load a CSV into a Pandas DataFrame
- [ ] Identify and handle missing values
- [ ] Group data and perform aggregations
- [ ] Convert cleaned data to Parquet
- [ ] Write a Python script to upload to AWS S3 using Boto3

### 📄 Project
**Title:** CSV → Clean Parquet → S3 Upload
**Deliverables:**
- `csv_to_parquet_to_s3.py`
- Documented steps in `README.md`
- Notes in `notes.md`

### 📝 Progress Log (`notes.md`)
Use this to track:
- What you’re learning
- Errors or blockers you encounter
- Questions or assumptions to revisit
- Snippets, tricks, and gotchas

---

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

---

## 🧱 Module 3: Analytics Engineering & Warehousing

### 🧠 Overview
This module focuses on the transformation layer between raw data and analysis-ready outputs. You'll use tools like dbt to build structured, reliable, and documented data models. You’ll also explore data warehouse platforms and optimisation strategies.

### 📚 References
- dbt documentation: https://docs.getdbt.com/
- *Designing Machine Learning Systems* — Chip Huyen (Ch. 5 on data tooling)
- *Fundamentals of Data Engineering* — Joe Reis & Matt Housley (Ch. 6–7 on modeling and warehousing)
- BigQuery docs: https://cloud.google.com/bigquery/docs
- *Effective Pandas* — Matt Harrison (joins, reshaping for staging layers) (joins, reshaping for staging layers)

### 🧪 Tasks & Exercises
- [ ] Create a dbt project and connect it to a sample warehouse (e.g. BigQuery)
- [ ] Build staging models to clean raw input tables
- [ ] Create intermediate and final models using `ref()` and `config`
- [ ] Write and compile documentation using dbt docs
- [ ] Implement table partitioning or incremental models

### 📄 Project
**Title:** Analytics-Ready Data Warehouse Model
**Deliverables:**
- A working dbt project with at least 3 models (staging → core → reporting)
- A warehouse structure visible in BigQuery/Snowflake/Redshift
- Screenshots of compiled dbt docs
- Notes and learnings in `notes.md`

### 📝 Progress Log (`notes.md`)
Use this to track:
- How dbt’s transformation layers work
- Naming conventions and testing strategies
- Warehouse setup steps and cloud config tips
- Notes on performance tuning, indexing, or costs

---

## 🤖 Module 4: Core Data Science & ML Principles

### 🧠 Overview
This module focuses on foundational data science and machine learning concepts. Inspired by *Data Science from Scratch*, it guides us through building core ML models from the ground up, reinforcing our understanding of how they work. We’ll also contrast our implementations with scikit-learn equivalents to solidify applied fluency.

### 📚 References
- *Data Science from Scratch* — Joel Grus (entire book)
- *Hands-On Machine Learning* — Aurélien Géron (Chapters on model training/evaluation)
- scikit-learn documentation: https://scikit-learn.org/stable/user_guide.html
- Python Standard Library: https://docs.python.org/3/library/

### 🧪 Tasks & Exercises
- [ ] Manually implement linear regression from scratch (using lists and functions)
- [ ] Build k-Nearest Neighbours classifier using basic Python structures
- [ ] Create a decision tree using recursion and dictionaries
- [ ] Load a real dataset and train the same models using scikit-learn
- [ ] Compare performance between scratch and sklearn versions using metrics

### 📄 Project
**Title:** Core ML Models: From Scratch to Application
**Deliverables:**
- Python scripts for each implementation: `linear_regression.py`, `k_nearest_neighbors.py`, `decision_trees.py`
- Notebooks comparing those with sklearn: `ml_practice_notebooks/`
- `README.md` with theory explanations and reflections

### 📝 Progress Log (`core_concepts_notes.md`)
Use this to track:
- Concepts from each *Data Science from Scratch* chapter
- Implementation challenges
- Design decisions (e.g., recursive vs iterative logic)
- Accuracy gaps or performance differences

---

## ⚙️ Module 5: Deployment & Capstone

### 🧠 Overview
This module brings everything together — deploying your data pipelines or ML models into environments where others can access or interact with them. It introduces version control, containerisation, automation, and basic DevOps concepts to help you productionise and share your work.

### 📚 References
- Docker documentation: https://docs.docker.com/
- GitHub Docs: https://docs.github.com/
- *Designing Machine Learning Systems* — Chip Huyen (Ch. 7–9 on deployment and monitoring)
- MkDocs: https://www.mkdocs.org/
- Streamlit: https://streamlit.io/

### 🧪 Tasks & Exercises
- [ ] Dockerise a Python script or notebook
- [ ] Create a `requirements.txt` and Dockerfile
- [ ] Push code to GitHub and practice branching/merging
- [ ] Add logging to an ETL/ML pipeline
- [ ] Build a simple Streamlit or CLI dashboard from model output

### 📄 Project
**Title:** Deployable Data Product (Pipeline, ML Model, or Dashboard)
**Deliverables:**
- A working Docker image
- Deployed code pushed to GitHub
- `README_project.md` with install/run instructions
- If applicable, dashboard or notebook interface

### 📝 Progress Log (`notes.md`)
Use this to track:
- Docker/CLI config or networking issues
- Git usage improvements and hiccups
- Deployment blockers or cloud lessons
- Notes on versioning, reproducibility, and feedback handling

---

