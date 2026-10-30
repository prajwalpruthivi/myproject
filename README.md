
# myproject
# My FastAPI Project

A simple REST API built with **Python** and **FastAPI**, served with **Uvicorn**. This is my first backend project, created to learn API development, routing, and Git/GitHub workflow.

## Tech Stack

- Python 3.9
- FastAPI
- Uvicorn
- uv (Python package and project manager)
- Git & GitHub
- Visual Studio Code

## Features

- REST API built with FastAPI
- `GET /` endpoint that returns a JSON response
- Automatic interactive API documentation (Swagger UI)

## Project Structure

```
myproject/
├── main.py            # FastAPI application
├── pyproject.toml     # Project configuration and dependencies
├── uv.lock            # Locked dependency versions
├── src/myproject/     # Package folder
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/prajwalpruthivi/myproject.git
cd myproject
```

### 2. Create a virtual environment and install dependencies

```bash
uv venv
uv pip install "fastapi==0.115.0" "pydantic==2.9.2" "pydantic-core==2.23.4" uvicorn
```

> Note: these versions are used because Python 3.9 does not work with the newest Pydantic release. If you use Python 3.10 or newer, you can install the latest versions.

### 3. Run the server

On Windows:

```bash
.\.venv\Scripts\python.exe -m uvicorn main:app --host 127.0.0.1 --port 8081
```

On macOS / Linux:

```bash
.venv/bin/python -m uvicorn main:app --host 127.0.0.1 --port 8081
```

## API Documentation

After the server starts, open:

| Page | URL |
| --- | --- |
| Swagger UI | http://127.0.0.1:8081/docs |
| OpenAPI JSON | http://127.0.0.1:8081/openapi.json |

## Example Request

```bash
curl http://127.0.0.1:8081/
```

## What I Learned

- Setting up a Python project with `uv`
- Creating API endpoints with FastAPI
- Running an app with Uvicorn
- Reading automatic Swagger documentation
- Fixing a Python/Pydantic version mismatch
- Pushing a project to GitHub

## Future Improvements

- Add more endpoints (CRUD)
- Connect a database
- Add authentication
- Write tests

## Author

**Prajwal**
GitHub: [@prajwalpruthivi](https://github.com/prajwalpruthivi)
