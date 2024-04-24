
# Backend Documentation

This document provides an overview of the `backend` folder in the project.

## Overview

The backend of this project is built using Quart, a Python framework for asynchronous web applications. The backend code is stored in the `app/backend` folder.

## Structure

The `backend` folder is structured as follows:

- `app/backend/approaches`: This folder contains the classes powering the Chat and Ask tabs. Each class uses a different RAG (Retrieval Augmented Generation) approach.

- `app/backend/main.py`: This is the main entry point of the backend application.

- `app/backend/routes.py`: This file defines the routes for the backend application.

- `app/backend/utils.py`: This file contains utility functions used across the backend application.

## Dependencies
## Dependencies

The following packages are required:

- `Quart`: This is the Python framework used for building the backend of this project. It is an asynchronous web microframework for Python.

- `Hypercorn`: This is an ASGI server that is used to serve the Quart application.

- `gunicorn`: This is a WSGI HTTP server for Python web applications.

- `SQLAlchemy`: This is a SQL toolkit and Object-Relational Mapping (ORM) system for Python, which provides a full suite of well known enterprise-level persistence patterns.

- `psycopg2-binary`: This is a PostgreSQL adapter for Python. It is used to interface with the PostgreSQL database.

- `alembic`: This is a database migration tool for SQLAlchemy.

- `python-dotenv`: This package is used to read key-value pairs from a .env file and set them as environment variables.

- `pytest`: This is a testing framework for Python that is used to write simple, scalable tests.

- `pytest-asyncio`: This is a plugin for pytest that provides support for testing asyncio code.

- `httpx`: This is a fully featured HTTP client for Python with sync and async APIs.

- `pydantic`: This is a data validation library that uses Python type annotations.

Please note that the versions of these packages are specified in the `requirements.txt` file. To install these packages, run the following command in your terminal:

```sh
pip install -r app/backend/requirements.txt

## Key Files

### `main.py`

This file is the main entry point of the backend application. It sets up the Quart application and registers the routes.

### `routes.py`

This file defines the routes for the backend application. Each route corresponds to a different endpoint that the frontend can call.

### `utils.py`

This file contains utility functions used across the backend application. These functions are used for tasks such as error handling and data processing.

## Running the Backend

To run the backend, navigate to the `app/backend` directory and run the following command:

```sh
python3 main.py