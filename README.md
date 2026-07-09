# Fast Student API

A RESTful API built with FastAPI and Python for managing and retrieving student data.

## Tech Stack

- **Python 3.14**
- **FastAPI** — modern, high-performance web framework
- **Uvicorn** — ASGI server for running the app

## Getting Started

### Prerequisites

Make sure you have Python installed, then install dependencies:

```bash
pip install fastapi uvicorn
```

### Running the API

```bash
python -m uvicorn myapi:app --reload
```

The API will be available at `http://127.0.0.1:8000`

## Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Returns a welcome message |
| GET | `/get-student/{student_id}` | Returns data for a specific student by ID |

## Example Response

`GET /get-student/1`

```json
{
  "name": "jasmine",
  "age": 19,
  "class": "Year 2"
}
```

## Interactive Docs

FastAPI auto-generates interactive API documentation. Once the server is running, visit:

- **Swagger UI:** `http://127.0.0.1:8000/docs`
- **ReDoc:** `http://127.0.0.1:8000/redoc`

## Project Structure
