<h1 align="center">Vinícius Campos</h1>

<h3 align="center">AI & Data Platform Engineer</h3>

<p align="center">
  I design and build production-grade AI and data platforms, from LLM gateways, RAG systems, agents, and observability to lakehouse pipelines, cloud infrastructure, and cost-aware operations.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/vinicius-de-paula-monteiro-de-campos-128aa8189/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:viniciusdipaulla@icloud.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>

---

## What I Build

I work at the intersection of **applied AI systems**, **large-scale data platforms**, and **cloud-native infrastructure**.

* **LLM platforms:** multi-provider gateways, fallback routing, tool calling, agents, RAG, model serving, request telemetry, and token-level cost metering.
* **AI reliability:** agent reliability harnesses, grounded generation, RAG evaluation, LLM-as-judge workflows, regression gates in CI, MCP tooling, observability, and cost attribution.
* **Data platforms:** lakehouse architectures, batch and streaming pipelines, CDC ingestion, orchestration, schema-as-code, lineage, governance, and analytical workloads.
* **Cloud platforms:** infrastructure as code, containers, serverless workloads, CI/CD, observability, reliability engineering, and production operations across AWS, Azure, and GCP.

---

## AI Flagship Projects

### [agent-evals](https://github.com/camposvinicius/agent-evals)

<p>
  <img src="https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white" alt="Anthropic">
  <img src="https://img.shields.io/badge/Amazon%20Bedrock-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="Amazon Bedrock">
  <img src="https://img.shields.io/badge/MCP-1C1C1C?style=flat-square" alt="MCP">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

Reliability harness for **tool-calling agents**. It runs a real agent against frontier models and measures whether it stays grounded, refuses when it should, and avoids hallucinating, with cost and latency.

**Highlights**

* Production-shaped tool-calling agent (bounded loop, per-tool timeouts, citation-enforced grounding, explicit refusal and clarify)
* Tools served natively over **MCP**, the Model Context Protocol
* Live multi-model comparison across Claude Opus 4.8, Opus 4.7, Sonnet 4.6, and Haiku 4.5 on AWS Bedrock, with real cost and latency
* Outcome and trajectory metrics (grounding, hallucination, refusal, tool accuracy) gated in CI
* Surfaces where smaller models break, for example Haiku's hallucination rate jumps on ambiguous queries while the larger models hold

**Stack:** Python · Anthropic · AWS Bedrock · MCP · GitHub Actions

---

### [llm-gateway](https://github.com/camposvinicius/llm-gateway)

<p>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI">
  <img src="https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white" alt="Anthropic">
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini">
  <img src="https://img.shields.io/badge/Amazon%20Bedrock-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="Amazon Bedrock">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus">
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana">
</p>

Production-style **multi-provider LLM gateway** designed for cost-aware and observable AI workloads.

**Highlights**

* Unified API for OpenAI, Gemini, Anthropic, and Amazon Bedrock
* Fallback routing across providers
* Token-level cost metering using integer micro-USD
* Append-only usage ledger for auditability
* Unified tool-calling interface
* Metered web research agent
* Prometheus metrics and Grafana dashboards
* Designed around production concerns: observability, cost attribution, and reliability

**Stack:** Python · FastAPI · OpenAI · Anthropic · Gemini · Amazon Bedrock · Prometheus · Grafana

---

### [rag-evals](https://github.com/camposvinicius/rag-evals)

<p>
  <img src="https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white" alt="Anthropic">
  <img src="https://img.shields.io/badge/Amazon%20Bedrock-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="Amazon Bedrock">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

CI-friendly **RAG evaluation framework** focused on retrieval quality, faithfulness, and regression control.

**Highlights**

* Retrieval evaluation metrics
* LLM-as-judge faithfulness checks
* CI regression gate that fails the build when quality drops
* Designed for repeatable RAG quality validation
* Useful for preventing silent degradation in AI applications

**Stack:** Python · BM25 · AWS Bedrock · GitHub Actions

---

## Current Focus

* Building reliable **LLM gateways** for production AI workloads
* Designing **RAG systems** with evaluation, grounded generation, and quality gates
* Creating **cost-aware AI infrastructure** with telemetry, metering, and observability
* Applying **platform engineering practices** to AI and data systems
* Engineering **lakehouse platforms** with Spark, Iceberg, Delta Lake, Snowflake, and Databricks

---

## Core Stack

### AI & LLM

<p align="center">
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI">
  <img src="https://img.shields.io/badge/Anthropic-191919?style=flat-square&logo=anthropic&logoColor=white" alt="Anthropic">
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini">
  <img src="https://img.shields.io/badge/Amazon%20Bedrock-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="Amazon Bedrock">
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain">
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square" alt="LangGraph">
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="Hugging Face">
  <img src="https://img.shields.io/badge/vLLM-111827?style=flat-square" alt="vLLM">
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square" alt="FAISS">
  <img src="https://img.shields.io/badge/OpenSearch-005EB8?style=flat-square&logo=opensearch&logoColor=white" alt="OpenSearch">
</p>

<p align="center">
  LLM gateways · agents · tool calling · RAG · model serving · grounded generation · LLM observability · cost metering
</p>

### Data Platforms

<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark">
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="PySpark">
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white" alt="Snowflake">
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white" alt="Databricks">
  <img src="https://img.shields.io/badge/Apache%20Iceberg-60A5FA?style=flat-square" alt="Apache Iceberg">
  <img src="https://img.shields.io/badge/Delta%20Lake-00ADD8?style=flat-square" alt="Delta Lake">
  <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" alt="Apache Airflow">
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Apache Kafka">
  <img src="https://img.shields.io/badge/DataHub-53389E?style=flat-square" alt="DataHub">
  <img src="https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white" alt="BigQuery">
</p>

<p align="center">
  Lakehouse architecture · medallion pipelines · CDC ingestion · orchestration · catalog & lineage · PII masking · multi-cloud migrations
</p>

### Cloud & Platform Engineering

<p align="center">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS">
  <img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square" alt="Azure">
  <img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="GCP">
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform">
  <img src="https://img.shields.io/badge/AWS%20CDK-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS CDK">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes">
  <img src="https://img.shields.io/badge/Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white" alt="AWS Lambda">
  <img src="https://img.shields.io/badge/EKS-FF9900?style=flat-square&logo=amazoneks&logoColor=white" alt="Amazon EKS">
  <img src="https://img.shields.io/badge/ECS-FF9900?style=flat-square&logo=amazonecs&logoColor=white" alt="Amazon ECS">
</p>

<p align="center">
  Infrastructure as code · containers · serverless · event-driven systems · OIDC CI/CD · production operations
</p>

### DevOps, Databases & Observability

<p align="center">
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
  <img src="https://img.shields.io/badge/GitLab%20CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white" alt="GitLab CI">
  <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white" alt="ArgoCD">
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white" alt="Jenkins">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus">
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana">
  <img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=flat-square&logo=amazoncloudwatch&logoColor=white" alt="CloudWatch">
</p>

<p align="center">
  CI/CD quality gates · alarms & dashboards · request tracing · cost attribution · DLQ/quarantine flows · production runbooks
</p>

### Programming

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/SQL-336791?style=flat-square" alt="SQL">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/HCL-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="HCL">
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" alt="Bash">
</p>

---

## Engineering Principles

* **Production-first design:** systems should be observable, testable, deployable, and operable.
* **Cost awareness by default:** especially for LLM workloads, cloud compute, storage, and data movement.
* **Reliability over demos:** fallback paths, retries, dashboards, alerts, and runbooks matter.
* **Evaluation-driven AI:** retrieval quality, faithfulness, grounded generation, and regression gates should be part of the workflow.
* **Data quality and governance:** schemas, lineage, masking, validation, and ownership should be part of the platform.
* **Automation and repeatability:** infrastructure, pipelines, and deployments should be reproducible through code.

---

## Data Engineering and Platform Projects

| Project                                                                                    | Focus                                                                                                                                | Stack                                    |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------- |
| [aws-snowflake-etl](https://github.com/camposvinicius/aws-snowflake-etl)                   | AWS-to-Snowflake data pipeline for analytical workloads, focused on cloud ingestion, transformation, and data warehouse integration. | Python · AWS · Snowflake · ETL           |
| [azure-etl](https://github.com/camposvinicius/azure-etl)                                   | Azure ETL pipeline ingesting external API data for analytical processing.                                                            | Azure · Python · ETL · APIs              |
| [aws-etl](https://github.com/camposvinicius/aws-etl)                                       | AWS ETL pipeline using open datasets and cloud storage patterns.                                                                     | AWS · Python · S3 · ETL                  |
| [gcp-etl](https://github.com/camposvinicius/gcp-etl)                                       | GCP ETL pipeline built around public data ingestion and processing.                                                                  | GCP · Python · ETL · BigQuery            |
| [vini-dataengineer](https://github.com/camposvinicius/vini-dataengineer)                   | Data engineering study projects across core pipeline patterns.                                                                       | Jupyter · Spark · SQL · Data Engineering |
| [vini-project-covid-data-BR](https://github.com/camposvinicius/vini-project-covid-data-BR) | Brazilian COVID data pipeline and analytics project.                                                                                 | Spark · Kafka · Jupyter · Analytics      |

---

## GitHub Stats

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=camposvinicius&show_icons=true&theme=react&include_all_commits=true&count_private=true" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=camposvinicius&layout=compact&langs_count=8&theme=react" alt="Top languages">
</div>

---

## Let's Connect

<p align="center">
  <a href="https://www.linkedin.com/in/vinicius-de-paula-monteiro-de-campos-128aa8189/" target="_blank">
    <img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn">
  </a>
  <a href="mailto:viniciusdipaulla@icloud.com">
    <img src="https://img.shields.io/badge/Send%20Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Send Email">
  </a>
</p>
