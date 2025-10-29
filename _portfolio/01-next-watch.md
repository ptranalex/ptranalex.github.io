---
title: "NextWatch"
excerpt: "A modern movie discovery platform powered by FastAPI, Next.js, and vector-based recommendations."
header:
  image: /assets/images/nextwatch-header.jpg
  teaser: /assets/images/nextwatch-teaser.jpg
sidebar:
  - title: "Role"
    text: "Technical Lead & Full Stack Developer"
  - title: "Tech Stack"
    text: "FastAPI, Next.js, Redis, Qdrant, AWS, GitHub Actions"
  - title: "Repository"
    text: "[GitHub](https://github.com/ptranalex/nextwatch)"
gallery:
  - url: /assets/images/nextwatch-1.jpg
    image_path: /assets/images/nextwatch-1.jpg
    alt: "Movie grid UI"
  - url: /assets/images/nextwatch-2.jpg
    image_path: /assets/images/nextwatch-2.jpg
    alt: "Recommendation view"
---

## Project Overview

**NextWatch** is a movie discovery platform designed to help users find what to watch next — powered by a custom vector-based recommendation engine.

The system combines structured movie metadata with semantic embeddings to provide personalized recommendations that go beyond genres or ratings.

---

## Key Features

- 🎬 **Vector Search Recommendations** — built with Qdrant and OpenAI embeddings
- ⚙️ **FastAPI Backend** — modular microservice architecture with caching and observability
- 💡 **Next.js Frontend** — optimized for fast browsing and responsive design
- 🧠 **LLM-Ready Design** — supports AI-assisted movie summaries and conversational search

---

## Architecture & Technologies

- **Backend:** FastAPI, PostgreSQL, Redis, Qdrant
- **Frontend:** Next.js, TypeScript, Tailwind CSS
- **Infra:** AWS EC2, GitHub Actions, Docker
- **Monitoring:** OpenTelemetry, Tempo

---

## Challenges & Solutions

### Challenge: Efficient Vector Search at Scale

Implemented **multi-layer caching (Redis + in-memory L1)** to keep search latency under 50 ms even with tens of thousands of vectors.

### Challenge: Data Consistency Across Services

Designed a shared core module (`movie-storage`) to unify data logic between importers, APIs, and frontends.

---

## Results

- 🚀 Search latency reduced by ~65%
- 🧠 Improved recommendation relevance (higher click-through in internal tests)
- 🧩 Modularized architecture for future ML extensions

---

## Lessons Learned

Building NextWatch reinforced the value of clean abstractions, strong observability, and balancing system design with product experience.

The next step: evolving it into a full recommendation API for multi-media content.

{% include gallery caption="Screens from NextWatch" %}

---

<!-- ## Links

- [Live Demo](https://alexsandbox.me)
- [GitHub Repository](https://github.com/ptranalex/nextwatch) -->
