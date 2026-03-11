
# Panagiotis Panageas

### Python Developer | Automation Systems | Computer Vision

![Python](https://img.shields.io/badge/Python-Developer-yellow?logo=python)
![Automation](https://img.shields.io/badge/Specialization-Automation-green)
![Computer Vision](https://img.shields.io/badge/Field-Computer%20Vision-blue)
![CUDA](https://img.shields.io/badge/GPU-CUDA-76B900?logo=nvidia)

Backend-focused developer interested in **system design, concurrency, and building modular software systems**.

Currently pursuing a **BSc in Computer Science at the Hellenic Open University**.

---

# Latest Update

## agent-pr-firewall (GitHub App PR Governance)

- Released `v0.1.1` with reporting hardening.
- Updated docs with troubleshooting (`401` webhook signature, `403` integration permissions), token requirements, and security hygiene notes.

Repository  
https://github.com/Archangel-77/agent-pr-firewall

---

# Featured Project

## Hutsix — Computer Vision Automation Platform

Hutsix is a **Windows desktop automation platform** written in **Python and PySide6**.

It automates repetitive keyboard and mouse workflows using a **profile-based visual system** built around trigger detection and deterministic action execution.

The platform combines:

* automation architecture
* computer vision pipelines
* GPU acceleration
* desktop application engineering

### Key Features

* modular trigger/action automation engine
* pixel, image and OCR detection
* profile-based automation workflows
* deterministic keyboard and mouse playback
* CUDA accelerated AI workflows
* real-time diagnostics and monitoring

Project scale: **~70,000 lines of Python code**

Repository
[https://github.com/Archangel-77/hutsix-public](https://github.com/Archangel-77/hutsix-public)

---
# Architecture Overview

```
                   +----------------------+
                   |      PySide6 UI      |
                   +----------+-----------+
                              |
                              v
                   +----------------------+
                   | Profile / Config     |
                   | Manager              |
                   +----------+-----------+
                              |
                              v
                  +-----------------------+
                  |     Trigger Engine    |
                  | HOTKEY | PIXEL        |
                  | IMAGE  | OCR          |
                  +----+-----------+------+
                       |           |
                       |           |
             GUI EVENT BUS         |
                       |           |
                       v           v
            +---------------------------+
            |        Action Layer       |
            | Keyboard / Mouse Binds   |
            +------------+--------------+
                         |
                         v
                +------------------+
                |   WinAPI Layer   |
                | Input Simulation |
                +--------+---------+
                         |
                         v
                +------------------+
                |   Action Executor|
                |  Deterministic   |
                | Input Playback   |
                +--------+---------+
                         |
                         v
             +----------------------------+
             | Watchdog Scheduler         |
             | Health & Performance Layer |
             +-------------+--------------+
                           |
                           v
                  +------------------+
                  | Diagnostics      |
                  | Monitoring       |
                  +------------------+
```

The system is designed as a **modular event-driven automation platform** with clear separation between detection, scheduling, execution and monitoring layers.

---

# Tech Stack

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?logo=python\&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?logo=c\&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=mysql\&logoColor=white)

### Frameworks & Libraries

![PySide6](https://img.shields.io/badge/PySide6-Qt-green)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv\&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-red?logo=pytorch)
![YOLOX](https://img.shields.io/badge/YOLOX-Computer%20Vision-blue)
![EasyOCR](https://img.shields.io/badge/EasyOCR-OCR-lightgrey)

### Technologies

![CUDA](https://img.shields.io/badge/CUDA-GPU%20Acceleration-76B900?logo=nvidia)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-AI-blue)
![Automation](https://img.shields.io/badge/Desktop-Automation-green)

### Tools

![Git](https://img.shields.io/badge/Git-F05032?logo=git\&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-black?logo=linux)
![Windows](https://img.shields.io/badge/Windows-0078D6?logo=windows)

---

Demo Video
https://www.youtube.com/watch?v=U0kk0Ldu5q4

---
# Projects

## Task Manager API

Backend REST API for task management systems.

Repository
[https://github.com/Archangel-77/task-manager-api](https://github.com/Archangel-77/task-manager-api)

Focus areas:

* REST API architecture
* backend task management logic
* structured application design

---

## Event Driven Task Engine

Thread-based event processing engine demonstrating backend concurrency patterns.

Repository
https://github.com/Archangel-77/event-driven-task-engine

Key concepts:

* producer–consumer architecture
* priority queues
* graceful shutdown handling
* structured logging
* deterministic concurrency

---

## Tennis Club Ranking System

Academic team project implementing ranking logic.

Repository
https://github.com/Archangel-77/Project_33-Tennis-Club-Ranking

Focus areas:

* ranking algorithms
* object-oriented system design
* business rule enforcement
* structured data management

---

# Low Level Development

Experience with performance-oriented workflows such as:

* building **OpenCV from source with CUDA support**
* configuring GPU accelerated computer vision environments
* integrating native C/C++ libraries into Python pipelines

---

# Development Environment

Typical development environment used for Hutsix.

Operating System
Windows 11

Hardware

* multi-core CPUs
* CUDA capable NVIDIA GPUs

Key runtime technologies

* CUDA
* OpenCV custom builds
* GPU inference pipelines

---

# Contact

YouTube
[https://www.youtube.com/@Hutsix](https://www.youtube.com/@Hutsix)

Discord
[https://discord.gg/Sr5WUmeY](https://discord.gg/Sr5WUmeY)
