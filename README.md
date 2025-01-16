# microservice
# Microservices Demo Application

This is a simple microservices-based web application demonstrating the use of Docker Compose.

## Services

*   **Frontend:** A simple HTML page served by Nginx.
*   **Backend:** A Python Flask API that retrieves data from Redis.
*   **Redis:** A Redis instance used as a data store.

## Prerequisites

*   Docker Desktop or Docker Engine installed.

## Setup and Deployment

1.  Clone the repository: `git clone <your_repository_url>`
2.  Navigate to the project directory: `cd microservices-app`
3.  Build and run the application: `docker-compose up -d --build`

## Inter-Service Communication

The frontend communicates with the backend via HTTP requests to `http://localhost:5000/data`. The backend communicates with Redis using the Redis Python client library.

## Stopping the Application

`docker-compose down`
