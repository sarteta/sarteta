## Santiago Arteta

Backend / DevOps / SRE engineer. Cordoba, Argentina.

Four years running infrastructure across two parallel tracks:
PostgreSQL DBA + DevOps at NetMonitor, and Lead SRE at SocialNet/Valida
(biometric identity SaaS for Banco Galicia and Supervielle, where I
took it through ISO 27001 and held 99.9% uptime through the AWS
migration). Lately also building the AI-infra layer that goes on top —
WhatsApp RAG bots for LATAM SMBs, MCP servers, eval harnesses for
LLM-driven systems.

Spanish first language, English C2 (EF SET 73/100, certified 2024).

### What I've been doing

- **Lead SRE / DevOps @ SocialNet S.A. (Valida)** — May 2025 → Apr 2026.
  5-engineer team. Drove the migration of a biometric identity platform
  to a Multi-AZ AWS architecture, full Terraform IaC for ISO 27001
  certification, GitLab CI/CD for deploys, CloudWatch + Grafana
  observability. Optimized RDS PostgreSQL across the migration window
  with no customer-visible downtime. FinOps reviews that cut idle-NAT
  + idle-EC2 spend ~20%. The cost-review work is what eventually got
  pulled out into `aws-cost-optimizer-cli`.
- **DBA & DevOps @ NetMonitor** — Jun 2022 → present (part-time).
  PostgreSQL administration, replication, performance tuning. Built a
  custom OTA versioning system in Node.js. GitLab CI/CD across
  AI-integrated projects. Custom SQL plugins for Grafana that the ops
  team uses daily.
- **Freelance** — Embedded/Industrial IoT at F.E.M (3 yrs, ESP32 +
  ESP-IDF + FreeRTOS over MQTT) and Web Dev (Nobis Salud, Volt Motors,
  CR Mayorista — WordPress + custom PHP/Node).

### Pinned projects

**SRE / Observability**

- [`slo-toolkit`](https://github.com/sarteta/slo-toolkit) — YAML SLO
  spec → Prometheus rules + Grafana dashboards. Multi-window
  multi-burn-rate alerts from the Google SRE workbook. 24 tests +
  promtool validation in CI.
- [`postgres-production-playbook`](https://github.com/sarteta/postgres-production-playbook) —
  Read-only diagnostic queries for Postgres + Python aggregator that
  emits a single Markdown report. CI runs against real Postgres 16 on
  every PR. The kind of script collection I reach for during incident
  retros.

**Infrastructure / FinOps**

- [`terraform-aws-web-stack`](https://github.com/sarteta/terraform-aws-web-stack) —
  3-tier web stack on AWS (VPC + ALB + ECS Fargate + RDS). Simple +
  production examples, CI validation, tfsec scan. Has a `nat_mode` knob
  because we were wasting ~$100/mo on dev NATs at Socialnet.
- [`aws-cost-optimizer-cli`](https://github.com/sarteta/aws-cost-optimizer-cli) —
  Read-only Python CLI. Scans an account for idle EC2, orphan EBS,
  oversized RDS, dev NATs, S3 without lifecycle policies. `boto3` +
  mock mode. Produces a CSV/Markdown you can paste into Jira.

**AI infrastructure**

- [`mcp-supabase-latam`](https://github.com/sarteta/mcp-supabase-latam) —
  Multi-tenant Model Context Protocol server (TypeScript). Spanish-
  first knowledge base for Claude Desktop / Cursor / Claude Code, with
  tenant isolation built into the tool definitions. Drop-in for
  freelancers running bots across multiple LATAM clients.
- [`pgvector-rag-starter`](https://github.com/sarteta/pgvector-rag-starter) —
  FastAPI + Python RAG reference. Drop-in pgvector schema with
  Row-Level Security policy template. Ships with deterministic mock
  embeddings so the pipeline runs end-to-end in CI without API keys.
- [`whatsapp-rag-eval-kit`](https://github.com/sarteta/whatsapp-rag-eval-kit) —
  YAML eval harness for WhatsApp RAG bots. Catches the failure modes
  that actually matter in production: wrong intent, hallucinated
  phrases, slow replies, blown token cost. Exit code != 0 on failure
  so it works as a CI regression gate.

**Integrations / automation**

- [`whatsapp-twilio-lead-router`](https://github.com/sarteta/whatsapp-twilio-lead-router) —
  Node/Express. Twilio SMS → intent classifier → WhatsApp auto-reply +
  Slack ping for hot leads. `npm run demo` exercises it without Twilio
  creds.
- [`claude-mls-wordpress-sync`](https://github.com/sarteta/claude-mls-wordpress-sync) —
  Python async diff-sync: MLS (RESO / Bridge / Spark) → WordPress
  Custom Post Type via REST. YAML-driven field mapping, atomic state
  store, dead-letter log.

### Stack

AWS (EC2, RDS, S3, VPC, IAM, CloudWatch, Route53, ACM, Secrets
Manager), Terraform, GitHub Actions, GitLab CI/CD, Docker, Linux.
Python (FastAPI, asyncio, psycopg, pydantic), Node.js (Express),
TypeScript. PostgreSQL (replication, performance tuning, Performance
Insights), MySQL, Redis. Observability: Prometheus, Grafana,
CloudWatch. AI infra: Anthropic Claude API, OpenAI API, MCP, pgvector,
Supabase, RAG patterns. Compliance: ISO 27001, IAM least-privilege.

### Hiring

Open to USD contract / freelance — currently looking for SRE /
Platform Engineer remote work for US/UK firms. ~40 hrs/week available
from May 5, 2026 (current contract closes Apr 30). GMT-3, full
overlap with US Eastern + UK morning. Spanish (native), English (C2),
Portuguese (conversational).

Find me on [Upwork](https://www.upwork.com/freelancers/~01a85ffa3165fb83c7),
[LinkedIn](https://www.linkedin.com/in/santiago-arteta/),
or any of the pinned repos.
