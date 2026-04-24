## Santiago Arteta

Backend / DevOps engineer. Córdoba, Argentina.

I mostly work at the intersection of AWS infra, backend APIs, and third-party
integrations (Twilio, WordPress, MLS feeds). Spanish first language,
English fine for work.

### What I've been doing

- **DevOps Team Lead @ Socialnet** (May 2025 → Apr 2026). Led a small DevOps
  team, owned AWS infra design and rollout, coordinated with vendors, and
  ran a rigorous NAT / idle-resource / rightsizing review that cut
  infrastructure cost noticeably (that review is what eventually became
  `aws-cost-optimizer-cli`).
- **DBA & Backend @ DCS S.A.** (Aug 2022 → present). Java + PostgreSQL +
  Node.js + Grafana. SQL plugins, query tuning, some production on-call.
- **Freelance web dev** (since Jan 2023). WordPress, CRUD apps,
  e-commerce, integrations. Upwork + direct clients.

### Pinned projects

**Infrastructure / DevOps**

- [`terraform-aws-web-stack`](https://github.com/sarteta/terraform-aws-web-stack) —
  3-tier web stack on AWS (VPC + ALB + ECS Fargate + RDS). Simple +
  production examples, CI validation. Has a `nat_mode` knob because we
  were wasting ~$100/mo on dev NATs at Socialnet.
- [`aws-cost-optimizer-cli`](https://github.com/sarteta/aws-cost-optimizer-cli) —
  Read-only Python CLI. Scans an account for idle EC2, orphan EBS,
  oversized RDS, dev NATs, S3 without lifecycle policies. `boto3` +
  mock mode. Produces a CSV/Markdown you can paste into Jira.

**Integrations / automation**

- [`whatsapp-twilio-lead-router`](https://github.com/sarteta/whatsapp-twilio-lead-router) —
  Node/Express. Twilio SMS in → rule-based intent classifier → WhatsApp
  auto-reply + Slack ping for hot leads. SQLite event log, idempotent
  on `MessageSid`, quiet-hours aware. `npm run demo` shows the flow
  without Twilio creds.
- [`claude-mls-wordpress-sync`](https://github.com/sarteta/claude-mls-wordpress-sync) —
  Python async diff-sync: MLS (RESO / Bridge / Spark / mock adapter) →
  WordPress Custom Post Type via REST. YAML-driven field mapping,
  atomic state store, dead-letter log.

### Stack

AWS (VPC, ECS Fargate, RDS, S3, CloudFront, IAM, Secrets Manager),
Terraform, GitHub Actions, Docker. Python (FastAPI, asyncio, pydantic),
Node.js (Express), Java, a bit of Go. PostgreSQL, SQLite, Redis,
DynamoDB. TypeScript, React, WordPress / PHP on the legacy side.
Twilio, Stripe, PayPal, WP REST, custom MLS feeds (RESO Web API),
webhooks, OAuth.

### Hiring

Open to USD contract / freelance. ~20 hrs/week, remote, UTC-3
(flexible for US hours). Spanish (native), English (professional),
Portuguese (conversational).

Find me on [Upwork](https://www.upwork.com/freelancers/~01a85ffa3165fb83c7) or
[LinkedIn](https://www.linkedin.com/in/santiago-arteta-4541a5211/).
For issues, PRs, or just questions, any of the pinned repos is fine.
