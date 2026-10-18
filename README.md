# Christian Kilgore

**Healthcare Data Engineering | Cloud Data Architecture | Pipeline Orchestration**

Senior healthcare data engineer with 15+ years in health plan and benefits data, including 7+ years building production pipelines and data platforms. I design governed lakehouses for payer data: medical and pharmacy claims, eligibility, prior authorization, utilization management, and FHIR clinical data.

Currently architecting a Microsoft Fabric lakehouse modernization (25+ production pipelines, 100K+ members) and production Apache Airflow orchestration for FHIR data.

---

### Featured projects

| Project | What it shows | Links |
|---|---|---|
| **Healthcare Cost & Utilization Intelligence Platform** | Release-aware medallion lakehouse over real CMS Medicare and CDC PLACES data (2,762 counties). Data contracts with error budgets, quarantine, write-audit-publish, 13 fault-injection scenarios, Airflow 3, dbt, and a weekly live refresh. | [Live dashboard](https://kilgorec1024.github.io/healthcare-cost-utilization-platform/) · [Repo](https://github.com/KilgoreC1024/healthcare-cost-utilization-platform) |
| **Clinical Data ETL with Apache Airflow** | Proof of concept: a TaskFlow DAG that loads synthetic FHIR-shaped data, with pre-load quality gates, an atomic idempotent refresh, post-load audits, and CI that runs the full DAG in Docker. | [Repo](https://github.com/KilgoreC1024/airflow-synthetic-clinical-etl) |
| **Prior-Authorization Checklist Agent** | Healthcare LLM application (Kelley MBA team project) that keeps policy retrieval, completeness checks, and financial calculations deterministic, uses the LLM only for reading and explaining, constrains outputs to JSON schemas, and escalates ambiguous cases to human review. | [Live demo](https://kilgorec1024.github.io/prior-auth-agent-demo/) · [Repo](https://github.com/KilgoreC1024/prior-auth-agent-demo) |

All portfolio projects use public or synthetic data. No PHI, no proprietary code.

---

### Stack

- **Engineering:** SQL · Python · Spark/PySpark · Apache Airflow · dbt · Fabric Data Factory · Azure Data Factory · Docker · GitHub Actions
- **Platforms:** Microsoft Fabric · Azure Synapse · Azure SQL · DuckDB · Hadoop
- **Healthcare data:** Claims (ICD-10, CPT, NDC) · Eligibility · Prior Auth / UM · FHIR · HIPAA
- **Practices:** Medallion architecture · Dimensional modeling · Incremental loading · Data contracts · Data quality gates · Data governance

---

### Background

MS, Computer Science (AI & Enterprise Computing), Lewis University · MBA, Business Analytics, Indiana University Kelley School of Business

[LinkedIn](https://linkedin.com/in/christianjkilgore)
