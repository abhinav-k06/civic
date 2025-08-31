Civic Reporting — Production-ready package
=========================================

This bundle includes a backend (Express + SQLite) and a frontend (React + Vite) with Dockerfiles and docker-compose.yml.
It is ready to run locally with Docker, or you can push to a container host that supports Docker Compose.

Quick local run (recommended from WSL / Linux filesystem):

1. Extract the zip, open a terminal in the project folder.
2. Build & run:
   docker compose up --build
3. Frontend will be available at: http://localhost:3000
   Backend API at: http://localhost:4000 (e.g. /api/ping)

Notes:
- The frontend container uses Nginx and proxies /api to the backend service inside Docker network.
- For production, replace SQLite with Postgres and store uploads in S3.
