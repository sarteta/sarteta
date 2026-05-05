## Santiago Arteta

**AI Infrastructure & MCP Engineer · Senior SRE/DevOps**

Argentina-based, 4 years building production cloud infra for high-traffic banking systems. Now focused on the layer where AI agents meet real data: MCP servers, RAG pipelines, agentic tooling for Postgres + AWS workloads.

Previously Lead SRE/DevOps at SocialNet (Valida — biometric identity SaaS for Banco Galicia + Banco Supervielle), led ISO 27001 migration with 99.9% uptime and 24/7 incident response.

Available immediately for remote contractor work. Dual Argentine + Spanish citizenship — no sponsorship needed for EU/US/LATAM clients.

### MCP / AI Infrastructure

- [`mcp-postgres-doctor`](https://github.com/sarteta/mcp-postgres-doctor) — MCP-native Postgres diagnostic server. 9 read-only tools, hard safety gate, Docker compose, GHCR image, 37 tests in CI.
- [`mcp-aws-cost-doctor`](https://github.com/sarteta/mcp-aws-cost-doctor) — MCP server: AWS cost-leak finder (idle EC2, orphaned EBS, unused EIPs, oversized RDS) for AI agents.
- [`mcp-cloudwatch-explorer`](https://github.com/sarteta/mcp-cloudwatch-explorer) — MCP server: CloudWatch metrics, alarms, log error filtering — read-only.
- [`mcp-supabase-latam`](https://github.com/sarteta/mcp-supabase-latam) — MCP server for LATAM SMB Supabase administration.
- [`pgvector-rag-starter`](https://github.com/sarteta/pgvector-rag-starter) — multi-tenant RAG reference on Postgres + pgvector.
- [`whatsapp-rag-eval-kit`](https://github.com/sarteta/whatsapp-rag-eval-kit) — YAML-driven evaluation harness for WhatsApp RAG bots.

> The MCP trio (`mcp-postgres-doctor` + `mcp-aws-cost-doctor` + `mcp-cloudwatch-explorer`) lets one Claude session triage a production stack — DB load, cloud spend, observability — in a single conversation.

### SRE / DevOps / Postgres

- [`slo-toolkit`](https://github.com/sarteta/slo-toolkit) — multi-window burn-rate alerts and Grafana dashboards from a YAML SLO spec.
- [`postgres-production-playbook`](https://github.com/sarteta/postgres-production-playbook) — diagnostic SQL queries and runbooks for PostgreSQL on-call work.
- [`terraform-aws-web-stack`](https://github.com/sarteta/terraform-aws-web-stack) — production-grade Terraform modules for 3-tier containerized AWS web stack (VPC + ALB + ECS Fargate + RDS Multi-AZ).
- [`aws-cost-optimizer-cli`](https://github.com/sarteta/aws-cost-optimizer-cli) — read-only audit CLI that flags 7 classes of AWS cost waste.
- [`s3-lifecycle-audit`](https://github.com/sarteta/s3-lifecycle-audit) — declared lifecycle intent vs live S3 account drift detection.

### Stack

![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic_Claude-D97757?logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?logo=anthropic&logoColor=white)

### What I bring

- **MCP servers in production** — designed safety boundaries (read-only enforcement), test coverage, developer-facing docs.
- **Banking-grade reliability** — ISO 27001 compliance, multi-bank production (Galicia + Supervielle).
- **Postgres deep dive** — replication, query tuning, bloat analysis, MCP-based diagnostics.
- **AWS IaC at scale** — Terraform modules, multi-AZ deployments, cost auditing.
- **Spanish/English C2** (EF SET 73/100) — ready for LATAM, EU, US clients.

---

📄 [Download CV (English, PDF)](https://github.com/sarteta/sarteta/raw/main/CV-Santiago-Arteta-EN.pdf)

📧 santiagoarteta@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/santiago-arteta/) · 🌐 [github.com/sarteta](https://github.com/sarteta)
