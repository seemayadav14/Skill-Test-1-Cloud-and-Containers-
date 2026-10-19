# Microservices Containerization Assessment

## Overview
This project containerizes Node.js microservices using Docker and Docker Compose.

## Services
- User Service: http://localhost:3000
- Product Service: http://localhost:3001
- Order Service: http://localhost:3002
- Gateway Service: http://localhost:3003

## Requirements
- Docker Desktop
- Docker Compose

## Setup
1. Open PowerShell in the submission folder.
2. Build and start the services:

   docker compose up --build -d

3. Check running containers:

   docker compose ps

## Testing
Run these commands in PowerShell:

- Invoke-RestMethod http://localhost:3000/health
- Invoke-RestMethod http://localhost:3001/health
- Invoke-RestMethod http://localhost:3002/health
- Invoke-RestMethod http://localhost:3003/health
- Invoke-RestMethod http://localhost:3003/api/users
- Invoke-RestMethod http://localhost:3003/api/products
- Invoke-RestMethod http://localhost:3003/api/orders

## Troubleshooting
- If a container fails, run: docker compose logs
- If a port is occupied, close the other application using it.
- Ensure Docker Desktop is running.
- Rebuild after changes with: docker compose up --build -d

## Screenshots
Save screenshots in the screenshots folder and include them here.

- Docker containers: screenshots/docker-containers.png
- Service health checks: screenshots/health-checks.png
- Gateway API responses: screenshots/gateway-responses.png

## GitHub
https://github.com/seemayadav14/Skill-Test-1-Cloud-and-Containers-
