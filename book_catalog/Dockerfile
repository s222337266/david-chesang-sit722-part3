# Dockerfile for book_catalog microservice
FROM python:3.11-slim

# Working Directory
WORKDIR /app

COPY ./requirements.txt .

RUN pip install -r requirements.txt

COPY ./app ./book_catalog

# Run the FastAPI application with uvicorn
CMD uvicorn book_catalog.main:app --host 0.0.0.0 --port 4000

