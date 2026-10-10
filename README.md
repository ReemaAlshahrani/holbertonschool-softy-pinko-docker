# Holberton School - Softy Pinko Docker

This repository contains the coursework and implementation for the Softy Pinko project, focusing on containerization, service orchestration, reverse proxy configuration, and horizontal scaling using Docker and Nginx.

## Project Overview by Task

### Task 0: Ubuntu Base Container
- Directory: `task0/`
- Objective: Introduction to Docker by building a basic container image using an Ubuntu base image.
- Key files: `Dockerfile`

### Task 1: Python and Flask Back-end
- Directory: `task1/`
- Objective: Setting up a Python environment inside a container and deploying a simple Flask API server.
- Key files: `Dockerfile`, `api.py` (exposes an endpoint returning text on port 5252).

### Task 2: Front-end Integration with Nginx
- Directory: `task2/`
- Objective: Structuring the project into distinct backend and frontend directories, and serving static frontend files using an Nginx container.
- Key files: `back-end/`, `front-end/`, `front-end/Dockerfile`, `front-end/softy-pinko-front-end.conf`.

### Task 3: Connecting Front-end and Back-end
- Directory: `task3/`
- Objective: Establishing communication between the frontend and backend containers via AJAX requests and configuring Flask-CORS to handle cross-origin restrictions.
- Key files: Updated `index.html` with dynamic content elements and JavaScript AJAX calls, updated `api.py` and `Dockerfile`.

### Task 4: Multi-Container Management with Docker Compose
- Directory: `task4/`
- Objective: Managing multiple container builds and lifecycles simultaneously using a composition configuration file.
- Key files: `docker-compose.yml`.

### Task 5: Reverse Proxy Server
- Directory: `task5/`
- Objective: Implementing an Nginx reverse proxy as the single external entry point to route traffic to either the static file server or the API backend, while closing direct external access to internal ports.
- Key files: `proxy/Dockerfile`, `proxy/proxy.conf`, updated `docker-compose.yml`, and updated `index.html`.

### Task 6: Horizontal Scaling and Load Balancing
- Directory: `task6/`
- Objective: Scaling backend container instances to handle increased load and using Nginx for round-robin load balancing.
- Key files: `2-api-servers.txt`.

