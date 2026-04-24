# Panagiotis Panageas

**Python Backend Developer · Solo founder of a commercial Python product · Based in Greece**

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](#)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](#)

📧 [panpanageas@gmail.com](mailto:panpanageas@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

---

## 📌 About

I'm a Python developer who has spent the last few years doing something most juniors haven't: **shipping a commercial software product, supporting real paying customers, and iterating on it for years.**

I started coding in 2022 and within a year had a commercial product with paying customers. Before that I spent 8 years as a Petty Officer in the Hellenic Navy — the kind of environment where logistics failures have real consequences and "it works on my machine" isn't an option. That background shapes how I approach software: operationally, not academically.

My main work is **[Hutsix](https://github.com/Archangel-77/hutsix-public)** — a Python desktop automation platform I designed, built, and sell through Gumroad. Running it end-to-end has taught me the things that don't fit in tutorials: release discipline, graceful failure handling, observability, backwards-compatible changes, and saying no to scope creep.

Alongside that, I build **Python backends** (FastAPI, async SQLAlchemy, PostgreSQL, Docker) and event-driven services. I'm now looking to bring that shipping mindset into a collaborative engineering team — remote or Greece-based.

---

## 🏢 Flagship: Hutsix

> A commercial Python desktop automation platform. 50+ paying customers since 2023, under active development.

| What it is | Why it matters |
|---|---|
| Stateful workflow engine with profile-based triggers | Real state machines, real transitions, real edge cases |
| Async event processing & queue-based action dispatch | Same patterns used in backend job queues |
| GPU-accelerated computer vision (OpenCV + PyTorch + CUDA) | Real-time image pipelines under latency constraints |
| Modular service boundaries + structured diagnostics | Built to be debugged, not just to run happy-path |
| Shipped to real users, actively supported | Proof I can build, ship, and maintain, not just prototype |

**Stack:** Python · PySide6 / Qt · OpenCV · PyTorch · CUDA · async processing · state machines
**Repo:** [hutsix-public](https://github.com/Archangel-77/hutsix-public) · **Product:** distributed via Gumroad

---

## 🛠️ Backend Work

The public projects below are where I practise the backend patterns I want to use day-to-day.

### [`task-manager-api`](https://github.com/Archangel-77/task-manager-api) — Async FastAPI Reference Implementation
FastAPI · async SQLAlchemy · Alembic · PostgreSQL · JWT · Docker · pytest

A deliberate showcase of FastAPI's async capabilities done right: fully async SQLAlchemy sessions, non-blocking endpoint handlers throughout, per-user ownership isolation, JWT auth, Alembic migrations from day one, Docker Compose, and a pytest suite covering auth, ownership, filtering, and CRUD. The kind of codebase I'd point a new teammate to as a baseline.

### [`agent-pr-firewall`](https://github.com/Archangel-77/agent-pr-firewall) — GitHub App / Webhook Service
TypeScript · Node.js · Octokit · GitHub Webhooks

A webhook-driven GitHub App that enforces pull-request policy and merge checks. Good demonstration of event-driven design and secure third-party API integration (signed webhooks, Octokit, scoped permissions).

### [`event-driven-task-engine`](https://github.com/Archangel-77/event-driven-task-engine) — Concurrency Engine
Python · threading · queues · pytest · GitHub Actions

Queue-backed task dispatch with priority execution, graceful shutdown, and a CI-integrated test suite. The patterns transfer directly to message-broker consumers (RabbitMQ, Redis Streams) and async worker pools.

---

## ⚓ Service Background

**Hellenic Navy · Petty Officer · Submarine Division · 2003–2011**

Eight years responsible for submarine logistics: managing critical supplies, coordinating with crew under operational pressure, and keeping systems running where mistakes are measured in consequences rather than tickets. It built habits that transferred directly into software — operational discipline, clear failure documentation, and a preference for systems that fail loudly over systems that fail quietly.

---

## 🧰 Core Stack

**Backend:** Python · FastAPI · Pydantic · SQLAlchemy (async) · Alembic · REST · JWT · OpenAPI
**Data:** PostgreSQL · Redis · SQLite · SQL (advanced) · query optimisation
**DevOps:** Docker · Docker Compose · GitHub Actions · pytest · Git · Linux
**Also:** TypeScript / Node.js · OpenCV · PyTorch · CUDA · PySide6 / Qt

---

## 🧭 How I work

- **Small commits, readable history.** I'd rather land 30 small commits than one big-bang dump.
- **Type-annotated, Pydantic-validated, tested.** If it isn't tested, I don't trust it.
- **Migrations from day one.** Schemas change; pretending they don't is how teams get stuck.
- **Observability before optimisation.** If I can't see it, I can't fix it.
- **Write for the next engineer.** That engineer is usually me in six months.

---

## 📫 Get in touch

I'm looking for **Python / backend roles** — remote or Greece-based. Happy to talk about FastAPI services, event-driven systems, or what it's like supporting a product you wrote yourself at 2am.

- **Email:** [panpanageas@gmail.com](mailto:panpanageas@gmail.com)
- **LinkedIn:** [panagiotis-panageas-017ba1213](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

---

<sub>Currently studying Computer Science at the Hellenic Open University (expected graduation 2028).</sub>
