# Rust CRUD API

A RESTful API built using Rust to perform basic CRUD (Create, Read, Update, Delete) operations with PostgreSQL as the database. This project uses Docker for containerized deployment and demonstrates clean code practices in Rust.

## Features
- CRUD operations for managing resources.
- PostgreSQL database integration.
- Dockerized for seamless setup and deployment.
- Easy to extend and customize.

## Technologies Used
- Rust
- PostgreSQL
- Docker & Docker Compose

## Prerequisites
Before starting, make sure you have:
- Docker and Docker Compose installed.
- Rust and Cargo (if you want to build locally).
- A PostgreSQL client (optional, for direct database inspection).

## Setup Instructions
1. Clone the Repository
```bash
git clone https://github.com/yourusername/rust-crud-api.git
cd rust-crud-api
```
2. Build and Run with Docker
- To containerize and run the application:
```bash
docker compose up --build
```
- This will:
  - Spin up a PostgreSQL database container.
  - Build and start the Rust application in another container.
- The API will be available at http://localhost:8080

## Testing
Use a tool like Postman or curl to test the endpoints.
- Example curl commands:
  - GET all users:
    ```bash
     curl -X GET http://localhost:8000/users
    ```
   - POST a new user
     ```bash
      curl -X POST http://localhost:8000/users \
     -H "Content-Type: application/json" \
     -d '{"name": "John Doe", "email": "johndoe@gmail.com"}'
     ```

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.
