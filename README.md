# 🚀 Kommuna Backend (NestJS)

A **real-time messaging backend system** built with NestJS, designed to handle scalable chat interactions, WebSocket communication, and concurrent users.

## 📖 Overview

**Kommuna** is a backend-focused project that simulates a modern chat system.
The goal is to build and stress-test a **high-performance messaging infrastructure** capable of handling:

- Real-time communication
- Concurrent users
- Message persistence
- Online/offline presence tracking

This project emphasizes **WebSockets**, **event-driven architecture**, and **state synchronization**.

## 🧱 Tech Stack

- **Framework:** NestJS
- **Language:** TypeScript
- **Auth:** JWT
- **Real-time:** WebSockets (Socket.IO or WS)
- **Database:** Postgres
- **ORM/ODM:** Typeorm

## ✨ Core Features

- 🔐 Authentication (JWT-based)
- 💬 1-on-1 Messaging
- 📃 Conversations List
- 🟢 Online / Offline Presence (WebSockets)
- 📎 Media Uploads _(optional)_

## 🧠 Key Concepts Covered

- WebSockets (real-time communication)
- Event-driven systems
- State synchronization
- Message persistence
- Scalable backend architecture

## 📅 Development Breakdown

### Week 1

- Authentication system
- User model/schema
- Conversations schema

### Week 2

- Messaging system
- WebSocket setup (presence tracking)
- Real-time message delivery

### Week 3

- Media upload (optional)
- Cleanup & optimization
- API refinement

## ⚙️ Project Setup

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd kommuna-server
```

### 2. Install dependencies

```bash
pnpm install
```

### 3. Setup environment variables

Create a `.env` file in the root:

```env
PORT=3000
JWT_SECRET=your_secret_key
DATABASE_URL=your_database_connection
```

## ▶️ Running the Application

```bash
# development
pnpm run start:dev

# production
pnpm run start:prod
```

## 🔌 WebSocket Gateway

This project uses WebSockets for:

- Real-time messaging
- User presence (online/offline)
- Event broadcasting

Make sure your frontend connects to the correct WebSocket endpoint.

## 🧪 Testing

```bash
# unit tests
pnpm run test

# e2e tests
pnpm run test:e2e

# coverage
pnpm run test:cov
```

## 📂 Suggested Project Structure

```
src/
│
├── auth/            # Authentication (JWT)
├── users/           # User module
├── conversations/   # Conversations logic
├── messages/        # Messaging system
├── gateway/         # WebSocket gateway
├── common/          # Shared utilities
└── config/          # Environment config
```

## 🚀 Deployment

To deploy:

```bash
pnpm run build
pnpm run start:prod
```

You can deploy using:

- Docker
- AWS / VPS
- NestJS Mau (optional)

## 🎯 Project Goal Recap

This project is designed to:

- Stress-test backend systems
- Simulate real-world chat architecture
- Build strong backend + real-time engineering skills

## 📌 Notes

- Focus heavily on **WebSockets** — this is the core of the project.
- Optimize for **performance and scalability**, not just functionality.
- Keep APIs clean and consistent.
