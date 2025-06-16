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
