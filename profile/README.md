# NEXUS-Foundry: Unified Cognitive Digital Twin Platform

**NEXUS-Foundry** is a System-of-Systems industrial intelligence platform designed to transition traditional foundry operations from reactive monitoring to predictive, AI-driven orchestration across **Melting, Pouring, and Quality** stages.


## Industrial Problem Statement

Traditional foundry monitoring is **reactive**. Defects often originate during high-heat melting and pouring phases but are only detected post-cooling, leading to:

- **High Scrap Rates:** Post-production rework and material waste  
- **Unplanned Downtime:** Critical furnace failures disrupting supply chains  
- **Energy Inefficiency:** Massive consumption without real-time optimization  
- **The "Experience Gap":** Over-reliance on operator intuition instead of institutionalized intelligence  

**NEXUS-Foundry bridges this gap** by embedding data-driven intelligence into a unified digital thread.


## Key Novelty: The "Cognitive" Edge

Unlike traditional dashboards, NEXUS addresses the human element of manufacturing through a **GenAI-powered Digital Assistant**.

### Contextual Natural Language Querying

> **Operator:** *"How will today's 5% humidity spike affect our scrap rate during the pouring phase?"*  
> **NEXUS:** *"Based on historical logs and current sensor data, humidity above 4% increases gas porosity risk by 12%. Recommendation: Increase degassing duration by 45 seconds."*

## Core Features

- **3D Visual Twin**  
  Real-time 3D visualization of furnace health and molding lines using **Three.js** and **React Three Fiber**.

- **Predictive Intelligence**  
  LSTM-based forecasting of furnace lining degradation (validated using **NASA Turbofan** and **UCI Industrial** datasets).

- **What-If Simulation Engine**  
  Virtual sandbox to test alloy compositions and temperature adjustments before physical pouring.

- **Explainable AI (XAI)**  
  Actionable, logic-based recommendations for shop-floor operators.

- **Universal Connectivity**  
  Hardware-agnostic integration via **MQTT** and **OPC-UA** industrial protocols.


## System Architecture

The platform follows a hierarchical **Digital Thread** architecture:

1. **Edge Layer (Shop Floor)**  
   Real-time data ingestion and localized inference for safety-critical triggers.

2. **Cloud Intelligence Hub**  
   Predictive modeling, physics-based simulations, and GenAI orchestration.

3. **Application Layer**  
   Next.js 3D Command Center for plant-level orchestration.


## Essential Tech Stack

### Frontend & Design

- **Next.js (SSR)** — High-performance dashboard framework  
- **Three.js / React Three Fiber** — Real-time 3D rendering  
- **Figma** — Professional UI/UX and system architecture design  

### Backend & Intelligence

- **FastAPI** — Asynchronous Python API engine  
- **PyTorch** — LSTM and neural network predictive models  
- **LangChain** — Cognitive assistant (RAG-based querying)  

### Data & Infrastructure

- **TimescaleDB** — Time-series industrial log storage  
- **PostgreSQL** — Asset metadata and digital birth certificates  
- **Docker** — Modular containerized deployment  


## Installation & Setup

### Prerequisites

- Docker & Docker Compose  
- Python 3.10+  
- Node.js 18+  

### Quick Start

1. Clone the repository:

```bash
git clone https://github.com/your-username/nexus-foundry-os.git
cd nexus-foundry-os
```
2.Launch via Docker Compose:

```bash
docker-compose up --build
```
3.Access the platform

Repository Structure:
```bash
nexus-foundry-os/
├── frontend/        # Next.js & Three.js Command Center
├── backend/         # FastAPI Intelligence Hub (REST + WebSockets)
├── ml_models/       # PyTorch predictive models
├── data/            # Sample datasets (NASA, UCI, Kaggle)
├── docker/          # Containerization scripts
└── docs/            # Architecture diagrams & design specs
```

## Architecture:
![Description](final.png)
