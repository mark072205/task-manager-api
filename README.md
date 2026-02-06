# Task Manager API

A REST API built with Symfony, API Platform, and Docker for managing tasks.

## Requirements
- Docker
- Git

## Setup Instructions

1. Clone the repository

git clone <your-repository-url>  
cd task-manager-api

2. Start Docker containers

docker compose up -d


3. Run database migrations

symfony console make:migration
symfony console doctrine:migrations:migrate

4. Start the Symfony server

symfony serve:start

## API Access

Once the server is running, open your browser and go to:

http://localhost:8000/api

This displays the API Platform documentation where you can:
- Create a task (POST)
- Update a task (PUT/PATCH)
- Mark a task as completed

## Database

Database name: task_manager_api

## Docker

The project runs using Docker with:
- PHP container (Symfony application)
- Database container

To check running containers:

docker ps
