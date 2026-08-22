# Tasks Flask CRUD API

A compact REST API for managing tasks, created to practice HTTP resources, CRUD operations and automated API checks with Python.

## Features

- Create, list, read, update and delete tasks.
- JSON request and response payloads.
- Explicit 404 responses for missing tasks.
- A small test suite using pytest and requests.

## API

| Method | Route | Purpose |
| --- | --- | --- |
| POST | /tasks | Create a task |
| GET | /tasks | List tasks |
| GET | /tasks/<id> | Read one task |
| PUT | /tasks/<id> | Update a task |
| DELETE | /tasks/<id> | Delete a task |

## Stack

- Python
- Flask
- pytest
- requests

## Running locally

```bash
pip install -r requirements.txt
python app.py
```

The API runs at `http://127.0.0.1:5000`. With the server running, execute:

```bash
pytest tests.py
```

The current implementation keeps data in memory, which keeps the project focused on HTTP and API behavior. A natural next step would be adding persistence and request validation.
