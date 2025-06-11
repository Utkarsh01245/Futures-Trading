# 🚀 Personalised Futures Trading Platform

A full-stack, microservices-based **personalised trading platform** built with **Node.js**, **TypeScript**, and modern tools. Designed for real-time execution, efficient order matching, and reliable data storage, this platform simulates a production-ready futures trading system with an in-memory matching engine, WebSocket updates, and Redis-based queuing.

---

## 🧰 Tech Stack

| Layer | Technology |
|-------|------------|
| **Language & Runtime** | Node.js 20, TypeScript |
| **Package Manager** | pnpm |
| **Frontend** | Next.js, React, [lightweight-charts](https://github.com/tradingview/lightweight-charts) |
| **API Server** | Express.js, Prisma ORM |
| **WebSocket Server** | WebSockets + Redis Pub/Sub |
| **Matching Engine** | In-memory orderbook & logic |
| **Job Queue** | BullMQ + Redis |
| **Archiving** | PostgreSQL via Prisma |
| **Cache & Messaging** | Redis (Pub/Sub + BullMQ) |
| **CI/CD** | GitHub Actions → Docker Image → VPS (DigitalOcean) |
| **Containerization** | Docker, Docker Compose |

---

## ⚙️ Getting Started

### ✅ Prerequisites

- [Node.js](https://nodejs.org/) v20+
- [pnpm](https://pnpm.io/)
- [Docker](https://www.docker.com/) & Docker Compose

### 🔧 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/futures-trading-platform.git
   cd futures-trading-platform

2. **Spin up services:**
   ```bash
   docker-compose up --build
3. **Install dependencies for local dev (if needed)**
   ```bash
   pnpm install
4. **Migrate Database**
   ```pnpm --filter apps/server prisma migrate dev
5. **Start Development**
   ```bash
   pnpm dev
