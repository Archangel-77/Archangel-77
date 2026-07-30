# Panagiotis Panageas

**Python backend engineer.** I build production systems, ship commercially, and support real users.

I specialize in turning messy real-world problems into reliable, observable systems — from maritime data pipelines to commercial desktop automation. Async-native, PostgreSQL-backed, and built to survive production.

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)](https://prometheus.io/)
[![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)](https://opencv.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![CUDA](https://img.shields.io/badge/CUDA-76B900?logo=nvidia&logoColor=white)](https://developer.nvidia.com/cuda-toolkit)
[![YOLOX](https://img.shields.io/badge/YOLOX-00BCD4?logo=keras&logoColor=white)](https://github.com/Megvii-BaseDetection/YOLOX)
[![OCR](https://img.shields.io/badge/OCR-FF6F00?logo=tesseract&logoColor=white)](https://github.com/tesseract-ocr/tesseract)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

[panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213) ·

---

## What I've actually shipped

**[Hutsix](https://github.com/Archangel-77/hutsix-public)** — A commercial Windows desktop automation platform I built solo and sell on Gumroad, with paying customers since 2023. It runs a stateful workflow engine with profile-based triggers and GPU-accelerated computer vision (OpenCV + PyTorch + CUDA) for real-time latency. Async queue dispatch handles reliable task execution. I own everything: architecture, distribution, and user support .

**[agent-pr-firewall](https://github.com/Archangel-77/agent-pr-firewall)** — a GitHub App that acts as a merge guardrail for teams using human + AI coding workflows. Verifies signed webhooks, evaluates PRs against configurable policies (secret pattern detection, protected paths, missing issue references, PR size, draft status), and publishes results as a required Check Run with a managed PR comment. Reduced accidental secret commits by 30% and cut average review cycle time from 18 min to 12 min. Shipped to v0.1.1 with a full release cycle and deployment hardening guide.

**[task-manager-api](https://github.com/Archangel-77/task-manager-api)** — a production-style FastAPI service with async SQLAlchemy, Alembic migrations, PostgreSQL, JWT auth, Docker Compose, and 90%+ pytest coverage. Non-blocking handlers, migration-first schema control, strict per-user ownership isolation. Built to demonstrate the patterns I actually use at work — not coverage theatre.

**[event-driven-task-engine](https://github.com/Archangel-77/event-driven-task-engine)** — a queue-backed concurrency engine in Python with priority scheduling and graceful shutdown. The worker reliability patterns here transfer directly to RabbitMQ and Redis Streams architectures.

**[Conductor](https://github.com/Archangel-77/conductor)** — a lightweight, production-grade async task queue for Python teams that don't need Redis. PostgreSQL-backed with exactly-once semantics, exponential backoff retry, dead letter queue, structured logging, Prometheus metrics, and health checks — all without a message broker. 100% asyncio, 400+ tasks/sec per worker throughput. Published to PyPI as `conductor-task-queue`, with Docker Compose, Kubernetes, and systemd deployment guides. The patterns here (polling-based dispatch, idempotent processing, circuit-ready architecture) are the same ones I use in production data pipelines.

---

## Production work (professional & commercial)

**Feedstream — AIS Data Pipeline** *(2024–present)*  
Real-time maritime data ingestion system: WebSocket ingestion → idempotent Postgres writes → Redis caching → FastAPI query service. Added retry and circuit-breaking logic (exponential backoff + jitter) to prevent upstream failures cascading downstream. Cursor-based pagination and TTL Redis caching cut API response times by 60% for high-volume queries. Full observability via Prometheus metrics and Grafana dashboards brought MTTR from >1 hour to <10 minutes. Deployed on Fly.io with GitHub Actions CI/CD.

**Hutsix** *(2023–present)*  
See above.

---

## Private commercial projects

**RenewalRadar** *(private repo)* — B2B SaaS for detecting customer renewal risk before churn. Combines account data, usage signals, billing status, and health scoring with AI-assisted next-best-action recommendations. Stack: Next.js, TypeScript, PostgreSQL, Prisma, Stripe, OpenAI, background jobs.

**Listing Copilot** *(private repo)* — real estate SaaS with AI listing generation, lead inbox workflows, analytics, and Stripe billing. Stack: Next.js, TypeScript, Prisma, PostgreSQL, Playwright, OpenAI, Resend.

**AI Pipeline Platform** *(private repo)* — distributed platform for dataset generation and model training with async workers and API-key-based multi-tenancy. Stack: FastAPI, Python, PostgreSQL, Redis, MinIO/S3, GitHub Actions.

**ReplyKit** *(private repo)* — Manifest V3 Chrome extension for reusable snippet management and page-aware insertion. Stack: TypeScript, Chrome APIs.

---

## Stack

| Category | Technologies |
|---|---|
| **Languages** | Python, TypeScript, SQL, Bash |
| **Backend** | FastAPI, Pydantic, SQLAlchemy (async), Alembic, asyncpg, aiohttp |
| **Data** | PostgreSQL 16, Redis 7, SQLite |
| **Infrastructure** | Docker, Docker Compose, GitHub Actions, Fly.io |
| **Observability** | Prometheus, Grafana, structured logging |
| **Testing** | pytest, pytest-asyncio, Playwright, Ruff, MyPy, pre-commit |
| **Vision / ML** | OpenCV, PyTorch, CUDA |
| **Desktop** | PySide6/Qt |
| **System design** | Event-driven architecture, queue-based workers, state machines, cursor pagination |

---

## Background

Eight years in the Hellenic Navy as a Petty Officer in the Submarine Division (2003–2011). High-stakes logistics and operations under pressure. It shaped how I engineer: clear ownership, loud failures, predictable recovery.

## Education

**B.Sc. Computer Science**
**B.SC. Applied Electronics**
---

## Open to roles

Looking for Python / backend engineering positions — remote or EU-based — where I can own systems end to end, from architecture through deployment and operations. If your team ships real products and cares about reliability, I'd like to talk.

---

📫 **Reach me:** [panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213) · 

![Profile views](https://komarev.com/ghpvc/?username=Archangel-77&color=blue&style=flat)
