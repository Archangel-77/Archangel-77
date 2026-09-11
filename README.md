# Panagiotis Panageas

**Python Backend Engineer** — building reliable, observable systems with async Python, PostgreSQL, and production-grade deployment practices.

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)](https://redis.io/)
[![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white)](https://prometheus.io/)
[![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)](https://opencv.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)](https://pytorch.org/)
[![CUDA](https://img.shields.io/badge/CUDA-76B900?logo=nvidia&logoColor=white)](https://developer.nvidia.com/cuda-toolkit)
[![YOLOX](https://img.shields.io/badge/YOLOX-00BCD4?logo=keras&logoColor=white)](https://github.com/Megvii-BaseDetection/YOLOX)
[![OCR](https://img.shields.io/badge/OCR-FF6F00?logo=tesseract&logoColor=white)](https://github.com/tesseract-ocr/tesseract)
[![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![Stripe](https://img.shields.io/badge/Stripe-635BFF?logo=stripe&logoColor=white)](https://stripe.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

[panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

---

## About

Python backend engineer focused on systems that stay predictable under load and failure. Work spans real-time data pipelines, a commercially sold desktop automation platform, open-source developer tooling, and full-stack SaaS — with an emphasis on reliability, observability, and maintainability. Core work is in async Python (FastAPI, SQLAlchemy, asyncio) backed by PostgreSQL, with TypeScript for SaaS and tooling projects.

---

## Flagships

Three systems I designed, built, and operate end to end. Each is public, deployed or distributed, and documented with its own architecture decisions and known limitations.

**[Hutsix](https://github.com/Archangel-77/hutsix-public)** — commercial Windows desktop automation platform, sold through a public storefront since 2023 (€29.99, 14 releases). A profile-based workflow engine with a trigger evaluator (global hotkeys, pixel, template matching, OCR, YOLOX models), a watchdog scheduler enforcing per-binding cooldowns, and a deterministic input executor behind a focus guard. Ships as an MSI with a SHA-256-hashed release manifest, license activation, and per-binding diagnostics that explain why any trigger did or did not fire. Python, PySide6, OpenCV, PyTorch, CUDA. Maintained end to end: architecture, packaging, distribution, and customer support.

**[Conductor](https://github.com/Archangel-77/conductor)** — PostgreSQL-backed async task queue for Python teams who don't want to run a broker, published to PyPI as [`conductor-task-queue`](https://pypi.org/project/conductor-task-queue/) (v0.2.0). Atomic claiming via `FOR UPDATE SKIP LOCKED`, retries with exponential backoff, a dead-letter queue, priority routing, recurring tasks, per-task-type circuit breakers, task dependencies, and a gRPC API for polyglot workers. Delivery is at-least-once with idempotent handlers — a distinction the README documents rather than glosses over.

**[feedstream](https://github.com/Archangel-77/feedstream)** — real-time AIS maritime ingestion and query service, [live on Fly.io](https://feedstream.fly.dev/). A WebSocket ingestion worker feeding idempotent PostgreSQL writes (`ON CONFLICT` dedup keys), Redis caching, and a FastAPI query API. Reconnect logic uses exponential backoff with jitter plus an in-process circuit breaker. Ships five architecture decision records, Prometheus/Grafana dashboards, request-ID tracing, structured JSON logs, and an explicit list of accepted trade-offs. Alembic migrations run in CI before each release, and a separate retention process purges expired rows.

---

## Other Projects

### Backend & Infrastructure

**[task-manager-api](https://github.com/Archangel-77/task-manager-api)** — Production-style FastAPI service with async SQLAlchemy, Alembic migrations, PostgreSQL, JWT authentication, Docker Compose, and 85%+ pytest coverage. Non-blocking handlers, migration-first schema management, and strict per-user ownership isolation.

**[event-driven-task-engine](https://github.com/Archangel-77/event-driven-task-engine)** — Queue-backed concurrency engine in Python with priority scheduling and graceful shutdown, built around a clean separation between dispatch and execution. The worker reliability patterns carry over directly to RabbitMQ and Redis Streams architectures.

**[project_x_public](https://github.com/Archangel-77/project_x_public)** — Distributed platform for dataset generation and model training. FastAPI job API, async dataset/training workers, Redis + PostgreSQL job backend with automatic fallback, API-key-based multi-tenancy, and S3/MinIO artifact storage with retention cleanup. CI and release-acceptance gates included.

### Developer Tooling

**[agent-pr-firewall](https://github.com/Archangel-77/agent-pr-firewall)** — GitHub App that acts as a merge guardrail for teams using human + AI coding workflows. Verifies signed webhooks, evaluates pull requests against configurable policies (secret pattern detection, protected paths, missing issue references, PR size, draft status), and publishes results as a required check run with a managed PR comment. Released to v0.1.1 with a full release cycle and a deployment hardening guide.

**[ollama-vscode-agent](https://github.com/Archangel-77/ollama-vscode-agent)** — Local-first VS Code extension that connects to Ollama for streaming chat, grounded workspace context, reviewed code edits (diff preview with explicit apply/reject), and approved terminal command execution.

### Web & E-commerce

**[django-digital-products](https://github.com/Archangel-77/django-digital-products)** — Production-ready Django 4.2 e-commerce platform for selling digital products directly to consumers: product management, cart and checkout, Stripe webhooks, automated file delivery, order management, an admin dashboard, Celery + Redis, and Docker Compose.

---

## Private Projects

- **RenewalRadar** *(private)* — B2B SaaS that detects customer renewal risk before churn. Combines account data, renewal dates, usage and support signals, billing status, and transparent health scoring with AI-assisted next-best-action recommendations into an operational dashboard. Stack: Next.js, TypeScript, PostgreSQL, Prisma, Stripe, OpenAI, background jobs.
- **Listing Copilot** *(private)* — Real estate SaaS for agents: property management, AI listing draft generation, public one-sheet sharing with lead capture, an inquiry inbox and follow-up queue, seller reports, usage limits, and Stripe billing. Stack: Next.js App Router, TypeScript, Prisma, PostgreSQL, Auth.js, OpenAI, Resend, Playwright.
- **AI Pipeline Platform** *(private; public counterpart [project_x_public](https://github.com/Archangel-77/project_x_public))* — Distributed platform for dataset generation and model training with async workers and API-key-based multi-tenancy. Stack: FastAPI, Python, PostgreSQL, Redis, MinIO/S3, GitHub Actions.
- **ReplyKit** *(private)* — Manifest V3 Chrome extension for reusable snippet management with page-aware variables and an on-page picker. No build step, JSON import/export, favorites-first sorting. Stack: TypeScript, Chrome APIs.
- **Hutsix (commercial source)** *(private)* — The private source repository behind the commercial Hutsix desktop automation product. Stack: Python, PySide6, OpenCV, PyTorch, CUDA, YOLOX.

---

## Stack

| Category | Technologies |
|---|---|
| **Languages** | Python, TypeScript, SQL, Bash, JavaScript |
| **Backend** | FastAPI, Pydantic, SQLAlchemy (async), Alembic, asyncpg, aiohttp, Django, DRF |
| **Data** | PostgreSQL 16, Redis 7, SQLite, Prisma |
| **Infrastructure** | Docker, Docker Compose, GitHub Actions, Fly.io |
| **Observability** | Prometheus, Grafana, structured logging |
| **Testing** | pytest, pytest-asyncio, Vitest, Playwright, Ruff, MyPy, pre-commit |
| **SaaS / Web** | Next.js, Stripe, Auth.js, OpenAI API, Resend |
| **Vision / ML** | OpenCV, PyTorch, CUDA, YOLOX, ONNX Runtime |
| **Desktop** | PySide6/Qt |
| **System design** | Event-driven architecture, queue-based workers, state machines, circuit breakers, cursor pagination, at-least-once delivery with idempotent handlers |

---

## Education

- B.Sc. Computer Science
- B.Sc. Applied Electronics

---

## Background

- Participated in Google Bootcamp 2022 as part of a team on project Ecodeorama.
- Currently working on FlameverseAI.

---

## Open to Roles

Open to Python / backend engineering positions — remote or EU-based — with end-to-end ownership from architecture through deployment and operations.

📫 **Contact:** [panpanageas@gmail.com](mailto:panpanageas@gmail.com) · [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

![Profile views](https://komarev.com/ghpvc/?username=Archangel-77&color=blue&style=flat)
