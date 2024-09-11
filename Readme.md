# Project Overview

This project showcases the versatility and power of Nginx in a modern web application architecture using Docker. It demonstrates how Nginx can be employed as a reverse proxy, load balancer, and static content server. The architecture includes:

- **Frontend**: Two frontend instances serving a React application.
- **Backend**: Two backend instances running a Spring Boot application.
- **Nginx**: Acts as a reverse proxy, load balancer, and static content server.

Nginx plays a crucial role in handling incoming requests, efficiently distributing them to the backend services, and serving static frontend files. Its robust configuration capabilities ensure smooth operation and scalability of the application.

## Project Structure

- **Docker**: Contains Dockerfiles for building frontend, backend, and Nginx images.
- **docker-compose.yml**: Configures and runs the multi-container Docker application.
- **nginx.conf**: Nginx configuration file for routing and load balancing.

## Prerequisites

- Docker
- Docker Compose

## Getting Started

### Clone the Repository

```bash
git clone <repository-url>
cd <project-directory>
```

### Build and Start the containers

Navigate to the docker directory (where docker-compose.yml is located) and run:

```bash
docker-compose up --build
```

### Access the app
Frontend: Access via http://localhost. Nginx will serve the frontend and manage communication with backend services.
Backend: Load balanced by Nginx and accessible via /api/ routes.

## File Descriptions

- **Dockerfile.backend**: Dockerfile for building the backend image.
- **Dockerfile.frontend**: Dockerfile for building the frontend image.
- **Dockerfile.nginx**: Dockerfile for building the Nginx image.
- **nginx.conf**: Configuration file to leverage Nginx’s capabilities for routing and load balancing.
- **docker-compose.yml**: File to define and run multi-container Docker applications, integrating Nginx with frontend and backend services.


