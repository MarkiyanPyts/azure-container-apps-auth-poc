# FastAPI API 1

A simple FastAPI application with hello world endpoint.

## Development (Local)

### Install dependencies
```bash
uv sync
```

### Run development server
```bash
uv run fastapi dev
```

### Run production server
```bash
uv run uvicorn main:app --host 0.0.0.0 --port 8000
```

## Docker

### Build and run with Docker Compose (Recommended)
```bash
docker-compose up --build
```

### Or build and run manually
```bash
# Build the Docker image
docker build -t fastapi-api-1 .

# Run the container
docker run -p 8000:8000 fastapi-api-1
```

### Stop the application
```bash
docker-compose down
```

## Endpoints

- `GET /` - Returns hello world message
- `GET /docs` - Swagger UI documentation
- `GET /redoc` - ReDoc documentation

## Access

The application will be available at:
- http://localhost:8000 - Main API endpoint
- http://localhost:8000/docs - Interactive API documentation