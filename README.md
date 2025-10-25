# Travel Management System

This repository contains a sample Travel Management System with a Spring Boot backend and a Vite/React frontend. The project is configured to run with Docker Compose for local development.

## Contents

- `carrental-backend-main/` - Java Spring Boot backend (uses MySQL)
- `carrental-frontend-main/` - React frontend (built with Vite)
- `docker-compose.yml` - Docker Compose file to run the full stack (MySQL, backend, frontend)

## Prerequisites

- Docker Desktop (Docker Engine + Docker Compose)
- Git

## Quick start (Docker Compose)

1. Open a terminal in the project root:

```powershell
cd C:\CloudDevops\Labproject
```

2. Build and start the services:

```powershell
docker-compose up --build -d
```

3. Check running containers:

```powershell
docker-compose ps
```

4. Stop the stack:

```powershell
docker-compose down
```

## Service ports (host -> container)

- Frontend: http://localhost:5173  (mapped 5173 -> 80)
- Backend: http://localhost:8082   (mapped 8082 -> 8081)
- MySQL:   localhost:3307          (mapped 3307 -> 3306)

## Database credentials

- MySQL root password: `Abhishek`
- Database name: `carrental`

> Note: These credentials are for local development only. Do not use them in production.

## Development notes

- The backend and frontend code are located in their respective folders. You can run them locally without Docker if desired.
- The `docker-compose.yml` includes a MySQL health check and configures the backend to wait until the database is healthy.

## GitHub

This repository is pushed to:

```
https://github.com/32342Abhishek/travel-management-system
```

## Contributing

If you'd like to contribute, fork the repo, make changes in a branch, and open a pull request.

---

If you'd like, I can also:
- Add a minimal CONTRIBUTING.md or LICENSE
- Add GitHub Actions for CI (build + test) — tell me which you'd prefer and I can scaffold it.
