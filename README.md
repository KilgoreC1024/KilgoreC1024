# Christian Kilgore

**Healthcare Data & AI Engineering | Cloud Platform Architecture | AI Reliability & Governance**

Senior healthcare data engineer with 15+ years in health plan and benefits data, including 7+ years building production pipelines and data platforms. I design governed lakehouses for payer data: medical and pharmacy claims, eligibility, prior authorization, utilization management, and FHIR clinical data.

Currently architecting a Microsoft Fabric lakehouse modernization (25+ production pipelines, 100K+ members). I also built production Azure Data Factory orchestration for FHIR clinical data; the [Airflow project](https://github.com/KilgoreC1024/airflow-synthetic-clinical-etl) below recreates that pattern on synthetic data, so you can run it without an Azure account.

My portfolio builds AI engineering on that foundation. Its centerpiece is an incident-investigation agent for healthcare data pipelines. It is evaluated against a deterministic baseline on incidents recorded from real pipeline runs, and the results are published, including where it fails.

---

### Featured projects

| Project | What it shows | Links |
|---|---|---|
| **Healthcare Data Reliability Copilot** | AI investigator for incidents in the cost platform and the clinical ETL below. Read-only tools, citations checked word for word against what it read, abstention when the evidence is thin, and fixes only as proposals a named person approves. Benchmarked against a deterministic playbook on 41 incidents recorded from real pipeline runs. On release 1 (30 incidents) the Claude agent got all 30 right, including three correct abstentions, with zero confident errors, for $2.74. On release 2 (11 harder incidents) it got 10 of 11; its one confident error was a silent unit change hidden behind a harmless alert, against the playbook's three. Failure analysis included. | [Live demo](https://kilgorec1024.github.io/healthcare-data-reliability-copilot/) · [Repo](https://github.com/KilgoreC1024/healthcare-data-reliability-copilot) · [Evaluation](https://github.com/KilgoreC1024/healthcare-data-reliability-copilot/blob/main/docs/evaluation.md) |
| **Healthcare Cost & Utilization Intelligence Platform** | Release-aware medallion lakehouse over real CMS Medicare and CDC PLACES data (2,762 counties). Data contracts with error budgets, quarantine, write-audit-publish, 13 fault-injection scenarios, Airflow 3, dbt, and a weekly live refresh. | [Live dashboard](https://kilgorec1024.github.io/healthcare-cost-utilization-platform/) · [Repo](https://github.com/KilgoreC1024/healthcare-cost-utilization-platform) |
| **Payer Claims Lakehouse** | Member-level claims lakehouse over CMS synthetic Medicare claims. Contract-gated yearly arrivals, versioned bronze, ICD-10 validation by fiscal year, exact member-months, and dbt gold marts for inpatient PMPM, admits and days per 1,000, and 30-day readmissions. CI rebuilds it from the public files and publishes the dashboard. | [Live dashboard](https://kilgorec1024.github.io/payer-claims-lakehouse-azure/) · [Repo](https://github.com/KilgoreC1024/payer-claims-lakehouse-azure) |
| **Clinical Data ETL with Apache Airflow** | Proof of concept: a TaskFlow DAG that loads synthetic FHIR-shaped data, with pre-load quality gates, an atomic idempotent refresh, post-load audits, and CI that runs the full DAG in Docker. The live demo runs the pipeline in your browser so you can break it with six fault scenarios, next to the latest Airflow run recorded in CI. | [Live demo](https://kilgorec1024.github.io/airflow-synthetic-clinical-etl/) · [Repo](https://github.com/KilgoreC1024/airflow-synthetic-clinical-etl) |
| **Prior-Authorization Checklist Agent** | Healthcare LLM application (Kelley MBA team project) that keeps policy retrieval, completeness checks, and financial calculations deterministic, uses the LLM only for reading and explaining, constrains outputs to JSON schemas, and escalates ambiguous cases to human review. | [Live demo](https://kilgorec1024.github.io/prior-auth-agent-demo/) · [Repo](https://github.com/KilgoreC1024/prior-auth-agent-demo) |

All portfolio projects use public or synthetic data. No PHI, no proprietary code.

---

### Stack

- **Engineering:** SQL · Python · Spark/PySpark · Apache Airflow · dbt · Fabric Data Factory · Azure Data Factory · Docker · GitHub Actions
- **AI engineering:** Claude API (agentic tool use, structured outputs) · LLM evaluation harnesses · Evidence grounding · Prompt-injection testing · Human-in-the-loop approval · OpenTelemetry tracing
- **Platforms:** Microsoft Fabric · Azure Synapse · Azure SQL · DuckDB · Hadoop
- **Healthcare data:** Claims (ICD-10, CPT, NDC) · Eligibility · Prior Auth / UM · FHIR · HIPAA
- **Practices:** Medallion architecture · Dimensional modeling · Incremental loading · Data contracts · Data quality gates · Data governance

---

### Background

MS, Computer Science (AI & Enterprise Computing), Lewis University · MBA, Business Analytics, Indiana University Kelley School of Business

[LinkedIn](https://linkedin.com/in/christianjkilgore)
