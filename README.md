# Panagiotis Panageas

**Python Backend Engineer** — building reliable, observable systems with async Python, PostgreSQL, and production-grade deployment practices.

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

[panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

---

## About

Python backend engineer focused on systems that stay predictable under load and failure. Experience spans real-time data pipelines, commercial desktop automation, and developer tooling, with an emphasis on reliability, observability, and maintainability. Work is primarily in async Python (FastAPI, SQLAlchemy, asyncio) backed by PostgreSQL.

---

## Professional Experience

**Feedstream — AIS Data Pipeline** *(2024–present)*  
Real-time maritime data ingestion system: WebSocket ingestion → idempotent PostgreSQL writes → Redis caching → FastAPI query service. Introduced retry and circuit-breaking logic (exponential backoff with jitter) to contain upstream failures and prevent them from cascading downstream. Cursor-based pagination and TTL-based Redis caching reduced API response times by 60% for high-volume queries. Added full observability via Prometheus metrics and Grafana dashboards, reducing mean time to recovery from over 1 hour to under 10 minutes. Deployed on Fly.io with GitHub Actions CI/CD.

**[Hutsix](https://github.com/Archangel-77/hutsix-public)** *(2023–present)*  
Commercial Windows desktop automation platform, built and sold independently since 2023. Runs a stateful workflow engine with profile-based triggers and GPU-accelerated computer vision (OpenCV, PyTorch, CUDA) for low-latency interaction, with reliable task execution via async queue dispatch. Maintained end to end — architecture, distribution, and customer support.

---

## Selected Projects

**[agent-pr-firewall](https://github.com/Archangel-77/agent-pr-firewall)** — GitHub App that acts as a merge guardrail for teams using human + AI coding workflows. Verifies signed webhooks, evaluates pull requests against configurable policies (secret pattern detection, protected paths, missing issue references, PR size, draft status), and publishes results as a required check run with a managed PR comment. Measured results: 30% fewer accidental secret commits and a reduction in average review cycle time from 18 to 12 minutes. Released to v0.1.1 with a full release cycle and deployment hardening guide.

**[task-manager-api](https://github.com/Archangel-77/task-manager-api)** — FastAPI service with async SQLAlchemy, Alembic migrations, PostgreSQL, JWT authentication, Docker Compose, and 90%+ pytest coverage. Non-blocking handlers, migration-first schema management, and strict per-user ownership isolation.

**[event-driven-task-engine](https://github.com/Archangel-77/event-driven-task-engine)** — Queue-backed concurrency engine in Python with priority scheduling and graceful shutdown. The worker reliability patterns carry over directly to RabbitMQ and Redis Streams architectures.

**[Conductor](https://github.com/Archangel-77/conductor)** — PostgreSQL-backed async task queue for Python teams that don't require a separate message broker. Provides exactly-once semantics, exponential backoff retry, a dead letter queue, structured logging, Prometheus metrics, and health checks. Fully asyncio, with measured throughput of 400+ tasks/sec per worker. Published to PyPI as `conductor-task-queue`, with Docker Compose, Kubernetes, and systemd deployment guides.

**Private commercial projects**

- **RenewalRadar** *(private repo)* — B2B SaaS that detects customer renewal risk before churn, combining account data, usage signals, billing status, and health scoring with AI-assisted next-best-action recommendations. Stack: Next.js, TypeScript, PostgreSQL, Prisma, Stripe, OpenAI, background jobs.
- **Listing Copilot** *(private repo)* — Real estate SaaS with AI listing generation, lead inbox workflows, analytics, and Stripe billing. Stack: Next.js, TypeScript, Prisma, PostgreSQL, Playwright, OpenAI, Resend.
- **AI Pipeline Platform** *(private repo)* — Distributed platform for dataset generation and model training with async workers and API-key-based multi-tenancy. Stack: FastAPI, Python, PostgreSQL, Redis, MinIO/S3, GitHub Actions.
- **ReplyKit** *(private repo)* — Manifest V3 Chrome extension for reusable snippet management and page-aware insertion. Stack: TypeScript, Chrome APIs.

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

## Education

- B.Sc. Computer Science (Ongoing)


---

## Background

- Participated in Google Bootcamp 2022 as part of a team on project Ecodeorama.
- Currently working on FlameverseAI.

---

## Open to Roles

Open to Python / backend engineering positions — remote or EU-based — with end-to-end ownership from architecture through deployment and operations.

📫 **Contact:** [panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

![Profile views](https://komarev.com/ghpvc/?username=Archangel-77&color=blue&style=flat)
