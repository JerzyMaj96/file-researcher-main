# File Researcher - Fullstack Deployment Hub

This repository serves as the **orchestration center** for the entire *File Researcher* project. It allows for the instant launch of the complete ecosystem (Frontend, Backend, Database, and Mailer) using Docker technology.

## System Architecture

The project consists of four independent microservices working together within an isolated Docker network:

1.  **Frontend**: React + Vite (Served via Nginx).
2.  **Backend**: Spring Boot 3 (Java 21) – REST API.
3.  **Database**: MySQL 8.0 – Persistent data storage.
4.  **Mail Server**: Mailpit – Development tool for testing email notifications.

## Quick Start (How to Run)

All images are pre-built and available on my **Docker Hub**, eliminating the need for manual code compilation.

**Prerequisites:** [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed.

### 1. Clone the repository
```bash
git clone [https://github.com/JerzyMaj96/file-researcher-main.git](https://github.com/JerzyMaj96/file-researcher-main.git)
cd file-researcher-main
```

### 2. Configure Environment Variables

Copy the template for environment variables (contains default test credentials):

```bash
cp .env.example .env
```

### 3. Launch containers
```bash
docker compose up -d
```

### 4. Access Services

Frontend UI: http://localhost:3000

Backend API: http://localhost:8080

Email Console (Mailpit): http://localhost:8025

### 5. Source code repositories

- Frontend: https://github.com/JerzyMaj96/fileresearcher-frontend
- Backend: https://github.com/JerzyMaj96/file-researcher-backend