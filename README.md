# Hi, I'm Santiago 👋

Backend / DevOps / full-stack engineer based in **Córdoba, Argentina** 🇦🇷

I build small, opinionated tools that solve a **specific problem well** —
usually at the intersection of **AWS infrastructure**, **backend APIs**,
and **integrations** (Twilio, WordPress, MLS feeds, webhooks).

---

## What I've been doing

**DevOps Team Lead @ Socialnet** — *May 2025 → Apr 2026*
Led a DevOps team, owned AWS infrastructure design & build, coordinated
with vendors, and **reduced infrastructure costs by running a rigorous
NAT / idle-resource / rightsizing review** (which eventually turned into
the `aws-cost-optimizer-cli` repo below).

**Database Admin & Backend Developer @ DCS S.A.** — *Aug 2022 → Present*
Java + PostgreSQL + Node.js + Grafana. SQL plugins, performance tuning,
production on-call.

**Freelance Web Dev** — *Jan 2023 → Present*
WordPress, CRUD apps, e-commerce, integrations. Upwork & direct clients.

---

## Pinned projects

### 🏗️ Infrastructure / DevOps

- **[terraform-aws-web-stack](https://github.com/sarteta/terraform-aws-web-stack)**
  — 3-tier containerised web stack on AWS (VPC + ALB + ECS Fargate + RDS
  Postgres). Ships with simple + production examples, CI validation, and
  a `nat_mode` knob that saves teams ~$100/mo on dev stacks.

- **[aws-cost-optimizer-cli](https://github.com/sarteta/aws-cost-optimizer-cli)**
  — Read-only Python CLI that scans an AWS account for cost leaks: idle
  EC2, orphan EBS, oversized RDS, dev NATs, S3 buckets with no lifecycle
  policy. `boto3` + a mock mode for demos. **18/18 tests pass**.

### 🔌 Integrations / automation

- **[whatsapp-twilio-lead-router](https://github.com/sarteta/whatsapp-twilio-lead-router)**
  — Node/Express service: Twilio SMS inbound → rule-first intent classifier
  (buyer / seller / investor / nurture / spam / STOP / HELP) → WhatsApp
  auto-reply + high-intent Slack notification. SQLite event log,
  idempotent via MessageSid, quiet-hours aware. **27/27 tests pass**,
  `npm run demo` shows the full flow without Twilio creds.

- **[claude-mls-wordpress-sync](https://github.com/sarteta/claude-mls-wordpress-sync)**
  — Python async diff-sync engine: pulls MLS listings (RESO / Bridge /
  Spark / mock adapter) → upserts into WordPress CPT via REST. YAML-
  driven field mapping, atomic state store, dead-letter logging.
  **13/13 tests pass**, `python -m src.sync --provider mock --dry-run`
  shows the engine.

---

## Stack

- **Cloud / infra:** AWS (VPC, ECS Fargate, RDS, S3, CloudFront, IAM,
  Secrets Manager), Terraform, GitHub Actions, Docker
- **Backend:** Python (FastAPI, asyncio, pydantic), Node.js (Express,
  ES modules), Java, Go (learning)
- **Data:** PostgreSQL, SQLite, Redis, DynamoDB
- **Frontend:** TypeScript, React, WordPress / PHP (legacy)
- **Integrations:** Twilio, Stripe, PayPal, WordPress REST, custom MLS
  feeds (RESO Web API), webhooks, OAuth

---

## Hiring me

I'm open to **USD contract / freelance** work.

- ⏱️ 20 hrs/week available
- 🌎 Remote, UTC-3 (flexible)
- 💬 Spanish (native), English (full professional), Portuguese
  (conversational)
- 🔗 [Upwork](https://www.upwork.com/freelancers/~01)  •  [LinkedIn](https://www.linkedin.com/in/santiago-arteta-4541a5211/)

Best way to reach me: **open an issue on any of the pinned repos**, or
ping me via Upwork.

---

<sub>This README is itself versioned in
[`sarteta/sarteta`](https://github.com/sarteta/sarteta). Every change is
a commit.</sub>
