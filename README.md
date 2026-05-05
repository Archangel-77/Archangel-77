# Panagiotis Panageas

**Python Backend Developer · Built and ships a commercial Python product · Based in Greece**

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](#)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](#)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](#)

📧 [panpanageas@gmail.com](mailto:panpanageas@gmail.com) · 💼 [LinkedIn](https://www.linkedin.com/in/panagiotis-panageas-017ba1213)

---

## 📌 About

I'm a Python developer who has spent the last few years doing something most juniors haven't: **shipping a commercial software product, supporting real paying customers, and iterating on it for years.**

I started coding in 2022 and within a year had a commercial product with paying customers. Before that I spent 8 years as a Petty Officer in the Hellenic Navy — the kind of environment where logistics failures have real consequences and "it works on my machine" isn't an option. That background shapes how I approach software: operationally, not academically. Small commits, typed and tested code, migrations from day one, and systems that fail loudly.

I'm currently looking to bring that shipping mindset into a collaborative engineering team — remote or Greece-based.

**Table of Contents**
- [About](#about)
- [Flagship: Hutsix](#flagship-hutsix)
- [Backend Work](#backend-work)
- [Other Builds (Private)](#other-builds-private)
- [Service Background](#service-background)
- [Core Stack](#core-stack)
- [Get in touch](#get-in-touch)
- [Contribution Guidelines](#contribution-guidelines)

I'm a Python developer who has spent the last few years doing something most juniors haven't: **shipping a commercial software product, supporting real paying customers, and iterating on it for years.**

I started coding in 2022 and within a year had a commercial product with paying customers. Before that I spent 8 years as a Petty Officer in the Hellenic Navy — the kind of environment where logistics failures have real consequences and "it works on my machine" isn't an option. That background shapes how I approach software: operationally, not academically. Small commits, typed and tested code, migrations from day one, and systems that fail loudly.

My main work is **[Hutsix](https://github.com/Archangel-77/hutsix-public)** — a Python desktop automation platform I designed, built, and sell through Gumroad. I build Python backends alongside it and I'm now looking to bring that shipping mindset into a collaborative engineering team — remote or Greece-based.

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Archangel-77&show_icons=true&theme=dark&hide_border=true&count_private=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Archangel-77&layout=compact&theme=dark&hide_border=true" height="150"/>
</p>

---

## 🏢 Flagship: Hutsix

> A commercial Python desktop automation platform. 50+ paying customers since 2023, under active development. **Challenges:** Overcoming real-time latency constraints in GPU-accelerated computer vision while maintaining stateful workflow reliability.

| What it is | Why it matters |
|---|---|
| **Stateful workflow engine** with profile-based triggers | Enables complex automation workflows with real state transitions and edge case handling |
| **Async event processing** & queue-based action dispatch | Implements patterns from backend job queues for reliable task execution |
| **GPU-accelerated computer vision** (OpenCV + PyTorch + CUDA) | Achieves real-time image processing under strict latency requirements |
| **Modular service architecture** + structured diagnostics | Designed for debuggability with clear service boundaries and failure diagnostics |
| **Shipped to real users** with active support | Demonstrates ability to build, maintain, and iterate on production software |

**Technical Stack:**
- **Core:** Python 3.11+ · PySide6 / Qt for GUI
- **Vision:** OpenCV 4.8 · PyTorch 2.0 · CUDA 12
- **Architecture:** Async processing · State machines · Queue-based dispatch
- **Deployment:** Dockerized · CI/CD with GitHub Actions

**Repo:** [hutsix-public](https://github.com/Archangel-77/hutsix-public) · **Product:** Distributed via Gumroad

---

## 🛠️ Backend Work

### [`task-manager-api`](https://github.com/Archangel-77/task-manager-api) — Async FastAPI Reference Implementation
FastAPI · async SQLAlchemy · Alembic · PostgreSQL · JWT · Docker · pytest

A deliberate showcase of FastAPI's async capabilities done right: fully async SQLAlchemy sessions, non-blocking endpoint handlers throughout, per-user ownership isolation, JWT auth, Alembic migrations from day one, Docker Compose, and a pytest suite covering auth, ownership, filtering, and CRUD. The kind of codebase I'd point a new teammate to as a baseline.

### [`agent-pr-firewall`](https://github.com/Archangel-77/agent-pr-firewall) — GitHub App / Webhook Service
TypeScript · Node.js · Octokit · GitHub Webhooks

A webhook-driven GitHub App that enforces pull-request policy and merge checks. Event-driven design with secure third-party API integration — signed webhooks, Octokit, scoped permissions.

### [`event-driven-task-engine`](https://github.com/Archangel-77/event-driven-task-engine) — Concurrency Engine
Python · threading · queues · pytest · GitHub Actions

Queue-backed task dispatch with priority execution, graceful shutdown, and a CI-integrated test suite. Patterns transfer directly to message-broker consumers (RabbitMQ, Redis Streams) and async worker pools.

---

## 🔒 Other Builds (Private)

Three additional commercial projects, currently private:

### **Listing Copilot** — Real Estate SaaS Platform
> Full SaaS solution for real estate agents with AI-powered listing copy generation and lead management.

**Key Features:**
- AI-generated listing copy using OpenAI API
- Lead inbox with email integration (Resend)
- Seller reports and analytics
- Stripe-based billing system
- Dockerized microservices architecture

**Tech Stack:**
- Frontend: Next.js · TypeScript
- Backend: Prisma · PostgreSQL
- DevOps: Docker · Playwright (testing)
- Integrations: OpenAI · Stripe · Resend

---

### **AI Pipeline Platform** — Distributed ML Infrastructure
> Network-deployed platform for dataset generation and model training.

**Key Features:**
- Distributed async workers with Redis
- Multi-tenant API key authentication
- Artifact storage with MinIO/S3
- CI/release gates for quality assurance

**Tech Stack:**
- Backend: FastAPI · Python 3.11
- Data: PostgreSQL · Redis
- DevOps: Docker · GitHub Actions
- Storage: MinIO/S3

---

### **ReplyKit** — Chrome Extension for Snippet Management
> Manifest V3 Chrome extension for managing reusable code snippets with on-page insertion.

**Key Features:**
- Page-aware variable substitution
- JSON import/export capabilities
- Secure storage with Chrome's API

**Tech Stack:**
- Chrome Extension: Manifest V3
- Frontend: TypeScript
- Storage: Chrome's secure storage API

## ⚓ Service Background

**Hellenic Navy · Petty Officer · Submarine Division · 2003–2011**

Eight years responsible for submarine logistics: managing critical supplies, coordinating with crew under operational pressure, and keeping systems running where mistakes are measured in consequences rather than tickets. It built habits that transferred directly into software — operational discipline, clear failure documentation, and a preference for systems that fail loudly over systems that fail quietly.

---

## 🧰 Core Stack

**Backend Development:**
- **Primary:** Python 3.11+ · FastAPI · Pydantic v2
- **ORM:** Async SQLAlchemy with Alembic migrations
- **Auth:** JWT-based authentication with OpenAPI documentation
- **Testing:** pytest framework with GitHub Actions CI

**Data Technologies:**
- **Databases:** PostgreSQL (primary) · Redis (caching) · SQLite (testing)
- **Optimization:** Advanced SQL query optimization techniques

**DevOps Infrastructure:**
- **Containerization:** Docker · Docker Compose
- **CI/CD:** GitHub Actions for automated testing and deployment
- **Testing:** pytest with comprehensive test coverage

**Additional Expertise:**
- **Frontend:** TypeScript / Node.js
- **Computer Vision:** OpenCV 4.8 · PyTorch 2.0 · CUDA 12
- **GUI Development:** PySide6 / Qt framework

## 📫 Get in touch

I'm looking for **Python / backend roles** — remote or Greece-based. Happy to talk about FastAPI services, event-driven systems, or what it's like supporting a product you wrote yourself at 2am.

**Preferred Communication Channels:**
- **Email:** [panpanageas@gmail.com](mailto:panpanageas@gmail.com) (preferred for initial contact)
- **LinkedIn:** [panagiotis-panageas-017ba1213](https://www.linkedin.com/in/panagiotis-panageas-017ba1213) (for professional networking)

**Ideal Candidates:**
- Experienced with async Python development
- Familiar with FastAPI and modern backend patterns
- Comfortable with DevOps tooling (Docker, GitHub Actions)
- Interested in shipping production-ready software

---

## 📝 Contribution Guidelines

1. **Code Quality:** All contributions must include type hints and pass the full test suite
2. **Branching:** Feature work should be done in separate branches with clear commit messages
3. **Testing:** Add tests for new features using pytest framework
4. **Documentation:** Update README.md and any relevant technical documentation
5. **Code Style:** Follow PEP8 guidelines with 2-space indentation
6. **PR Process:** Submit pull requests with detailed descriptions of changes
