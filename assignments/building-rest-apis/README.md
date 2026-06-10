# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Students will build a REST API using the FastAPI framework, learning how to define routes, handle requests, and return JSON responses.

## 📝 Tasks

### 🛠️ Set Up the API Server

#### Description
Create a basic FastAPI application with a health check endpoint.

#### Requirements
Completed program should:

- Install FastAPI and uvicorn
- Create a FastAPI app instance
- Define a `GET /health` endpoint that returns `{"status": "ok"}`

### 🛠️ Define Resource Endpoints

#### Description
Add CRUD endpoints for a resource (e.g., books, tasks, or students).

#### Requirements
Completed program should:

- Define a Pydantic model for the resource with at least 3 fields
- Implement `GET /items` to list all items
- Implement `POST /items` to create a new item
- Implement `GET /items/{id}` to retrieve a single item

### 🛠️ Data Validation and Error Handling

#### Description
Add input validation and proper error responses.

#### Requirements
Completed program should:

- Validate required fields using Pydantic
- Return 404 with a descriptive message when an item is not found
- Return 422 with validation details for invalid input

### 🛠️ Path Operations and Query Parameters (Stretch Goal)

#### Description
Add filtering and sorting capabilities via query parameters.

#### Requirements
Completed program should:

- Support `?category=` query parameter to filter items
- Support `?sort_by=` and `?order=` query parameters
- Document the API with auto-generated docs at `/docs`
