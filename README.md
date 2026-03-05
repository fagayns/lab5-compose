Lab 5 — Docker Compose Application

This project demonstrates a simple multi-service application using Docker Compose. It includes a backend service along with supporting services like a database and cache.
The application exposes several endpoints to verify that all services are working correctly.
## Run 
docker compose up --build 
(This command will: build the application images, create containers, start all services defined in docker-compose.yml)
## Endpoints
/health (Checks if the application is running.)
/db-test(Tests the connection to the database service.)
/cache-test(Tests the connection to the cache service.)
## Stop
- To stop all running containers:
docker compose down
- To also remove volumes:
docker compose down -v

Project Structure:

├── docker-compose.yml
├── Dockerfile
├── src/
│   └── application source code
└── README.md

