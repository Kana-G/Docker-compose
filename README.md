# Docker Compose Project

This project sets up a multi-service application using Docker Compose. The stack includes an Nginx reverse proxy, a Java-based web application, a React-based UI, and two Python services.

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- Docker
- Docker Compose

## Project Structure

The project directory contains the following files and directories:


## Services

### Nginx

Nginx is used as a reverse proxy to route traffic to the appropriate service.

- **Configuration**: `nginx/nginx.conf`

### Java Web Application

A Java-based web application running on an OpenJDK image.

- **Dockerfile**: `java-webapp/Dockerfile`

### React UI

A React-based user interface running on a Node.js image.

- **Dockerfile**: `react-ui/Dockerfile`

### Python Services

Two Python-based services running on a Python image with Flask.

- **Dockerfile**: `python-service1/Dockerfile`, `python-service2/Dockerfile`
- **Requirements**: `python-service1/requirements.txt`, `python-service2/requirements.txt`
- **Application**: `python-service1/app.py`, `python-service2/app.py`

## Setup

### Step 1: Clone the Repository

Clone this repository to your local machine:

```git clone [Docker-compose](https://github.com/Kana-G/Docker-compose)```

```cd Docker-compose```

### Step 2: Build and Start the Containers
Use Docker Compose to build and start all the containers:

```docker-compose up --build```
### Step 3: Access the Services
- Nginx (Reverse Proxy): http://localhost
- React UI: http://localhost:3000
- Java Web Application: http://localhost:8080
- Python Service 1: http://localhost:5000
- Python Service 2: http://localhost:5001

## Cleaning up
To stop and remove all the containers, networks, and volumes created by Docker Compose, run:

```docker-compose down```
