# Dockerfile for inventory_management microservice
FROM python:3.11-slim

# Working Directory
WORKDIR /app

COPY ./requirements.txt .

RUN pip install -r requirements.txt

COPY ./app ./inventory_management

# Run the FastAPI application with uvicorn
CMD uvicorn inventory_management.main:app --host 0.0.0.0 --port 4001

