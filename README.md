# Docker FastAPI Project

A containerized FastAPI application using Docker.

## Prerequisites

- Docker
- Docker Compose

## Project Structure

```
docker-fastapi-test/
├── data/
│   └── info.txt
├── Dockerfile
├── docker-compose.yml
└── README.md
```

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/SagarNikam09/docker-fastapi-test
cd docker-fastapi-test
```

2. Build and run the containers:
```bash
docker-compose up --build
```

3. Access the API:
- API documentation: http://localhost:8000/docs
- API endpoint: http://localhost:8000

## Development

- The API service runs on port 8000
- Data persistence is handled through volume mounting at `./data:/app/data`
- Auto-restart enabled unless manually stopped

## Commands

```bash
# Start containers
docker-compose up

# Stop containers
docker-compose down

# View logs
docker-compose logs api

# Rebuild containers
docker-compose up --build
```