## Santiago Arteta

**Senior SRE/DevOps · Postgres-focused tooling · MCP servers**

4 years operating production Postgres + AWS at SocialNet (Valida -- biometric identity SaaS, clients Banco Galicia + Banco Supervielle, ISO 27001 migration). Lead SRE/DevOps role through 2026-04. Now focused on open-source tooling for Postgres operations and MCP servers that plug AI agents into real production data.

Available for remote contractor work. Dual Argentine + Spanish citizenship -- no sponsorship needed for EU, US, or LATAM clients.

### Postgres operations (7 repos)

A cluster of tools that follow the order real Postgres incidents are resolved: rank cost, fix the top queries, validate migrations, watch autovacuum, drop dead indexes.

- [`pg-plan-lint`](https://github.com/sarteta/pg-plan-lint) -- lints EXPLAIN ANALYZE plans for anti-patterns (Seq Scan + Filter on big tables, Hash spilling to disk, Nested Loop on too many outer rows, planner row-estimate skew). JSON or text input.
- [`postgres-tuning-cookbook`](https://github.com/sarteta/postgres-tuning-cookbook) -- three patterns + CLI for the order Postgres tuning actually pays off: rank queries by cost, find autovacuum stalls, find unused indexes.
- [`postgres-migration-safety`](https://github.com/sarteta/postgres-migration-safety) -- 10-rule linter for migration files. Catches CREATE INDEX without CONCURRENTLY, ADD COLUMN NOT NULL without DEFAULT, ADD FK without NOT VALID, etc.
- [`postgres-incident-toolkit`](https://github.com/sarteta/postgres-incident-toolkit) -- live incident detection: long queries, lock waits, replication lag, bloat. Read-only.
- [`postgres-production-playbook`](https://github.com/sarteta/postgres-production-playbook) -- diagnostic SQL keyed to symptom (slow writes, disk filling, plan regressions, etc.)
- [`postgres-bloat-report`](https://github.com/sarteta/postgres-bloat-report) -- scans for bloated tables and indexes, reports estimated reclaimable bytes.
- [`mcp-postgres-doctor`](https://github.com/sarteta/mcp-postgres-doctor) -- the same scanners exposed over MCP, so a Claude session can run them mid-incident.

### MCP / AI infrastructure

- [`mcp-aws-cost-doctor`](https://github.com/sarteta/mcp-aws-cost-doctor) -- MCP server: AWS cost leaks (idle EC2, orphaned EBS, unused EIPs, oversized RDS).
- [`mcp-cloudwatch-explorer`](https://github.com/sarteta/mcp-cloudwatch-explorer) -- MCP server: CloudWatch metrics, alarms, log error filtering. Read-only.
- [`mcp-supabase-latam`](https://github.com/sarteta/mcp-supabase-latam) -- MCP server for LATAM SMB Supabase administration.
- [`pgvector-rag-starter`](https://github.com/sarteta/pgvector-rag-starter) -- multi-tenant RAG reference on Postgres + pgvector.
- [`whatsapp-rag-eval-kit`](https://github.com/sarteta/whatsapp-rag-eval-kit) -- YAML-driven evaluation harness for WhatsApp RAG bots.

### SRE / DevOps / IaC

- [`slo-toolkit`](https://github.com/sarteta/slo-toolkit) -- multi-window burn-rate alerts + Grafana dashboards from a YAML SLO spec.
- [`terraform-aws-web-stack`](https://github.com/sarteta/terraform-aws-web-stack) -- 3-tier containerized AWS web stack (VPC + ALB + ECS Fargate + RDS Multi-AZ).
- [`aws-cost-optimizer-cli`](https://github.com/sarteta/aws-cost-optimizer-cli) -- read-only audit CLI for 7 classes of AWS cost waste.
- [`s3-lifecycle-audit`](https://github.com/sarteta/s3-lifecycle-audit) -- declared lifecycle vs live S3 drift detection.

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

### What I do

- Postgres at production scale: pg_stat_statements, replication, autovacuum, query plan analysis. Six public repos in the cluster above.
- AWS IaC: Terraform modules, multi-AZ ECS/RDS, cost auditing, GitHub Actions pipelines.
- MCP servers as a real interface for AI agents to operate against production data, with read-only safety boundaries.
- Banking-grade compliance: ISO 27001 migration, 24/7 on-call rotation, SLO/SLI definition.
- English C2 (EF SET 73/100), Spanish native.

---

[CV English (PDF)](https://github.com/sarteta/sarteta/raw/main/CV-Santiago-Arteta-EN.pdf) · santiagoarteta@gmail.com · [LinkedIn](https://www.linkedin.com/in/santiago-arteta/) · [github.com/sarteta](https://github.com/sarteta)
