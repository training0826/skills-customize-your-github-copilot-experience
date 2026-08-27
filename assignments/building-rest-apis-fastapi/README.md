# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with the FastAPI framework. Practice defining routes, validating request data with Pydantic models, and implementing CRUD operations with clear HTTP responses.

## 📝 Tasks

### 🛠️ Create the FastAPI Application

#### Description

Create a Python application that starts a FastAPI server and provides a health-check endpoint. The endpoint should help a client confirm that the API is running.

#### Requirements

Completed program should:

- Create a FastAPI application.
- Define a `GET /health` route.
- Return a JSON response that includes a status such as `"ok"`.
- Start successfully with a command such as `uvicorn main:app --reload`.

### 🛠️ Add a Resource Endpoint

#### Description

Add an in-memory collection of resources, such as books, recipes, or students. Define a Pydantic model for the resource and create endpoints for listing resources and adding a new resource.

#### Requirements

Completed program should:

- Define a Pydantic model with at least three fields, including a unique identifier.
- Define a `GET /items` route that returns all stored resources as JSON.
- Define a `POST /items` route that accepts and validates a new resource.
- Return the newly created resource from the `POST /items` route.

### 🛠️ Implement CRUD Operations

#### Description

Complete the API by allowing clients to retrieve, update, and delete one resource at a time. Return an appropriate error when a requested resource does not exist.

#### Requirements

Completed program should:

- Define a `GET /items/{item_id}` route for retrieving one resource.
- Define a `PUT /items/{item_id}` route for updating an existing resource.
- Define a `DELETE /items/{item_id}` route for deleting an existing resource.
- Return a `404` response when the requested resource does not exist.
- Return appropriate success responses for successful retrieval, update, and deletion.
