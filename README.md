# Full-Stack Web Application (Next.js Frontend, FastAPI Backend)

This project is a full-stack web application consisting of a Next.js frontend and a FastAPI backend, containerized using Docker.

## Project Structure

-   **`frontend/`**: Contains the Next.js (TypeScript, Tailwind CSS) application.
    -   `frontend/README.md`: Instructions specific to the frontend development and build process.
-   **`backend/`**: Contains the FastAPI (Python) application.
    -   `backend/README.md`: Instructions specific to the backend development.
-   **`Dockerfile`**: Located in both `frontend/` and `backend/` directories, these files define the Docker images for each application.
-   **`docker-compose.yml`**: Located in the root directory, this file orchestrates the building and running of both frontend and backend services.

## Prerequisites

Before you begin, ensure you have the following installed on your system:
-   **Docker**: [Installation Guide](https://docs.docker.com/get-docker/)
-   **Docker Compose**: [Installation Guide](https://docs.docker.com/compose/install/) (Usually included with Docker Desktop)

## Getting Started with Docker Compose

This is the recommended way to run the application for a production-like environment or for easy setup.

1.  **Build the Docker Images:**
    Navigate to the root directory of the project and run:
    ```bash
    docker-compose build
    ```
    This command builds the Docker images for both the frontend and backend services as defined in their respective Dockerfiles and the `docker-compose.yml` file.

2.  **Run the Application:**
    Once the images are built, start the services using:
    ```bash
    docker-compose up
    ```
    This will start both the frontend and backend containers.
    -   The **Frontend** application will be accessible at [http://localhost:3000](http://localhost:3000).
    -   The **Backend** API will be accessible at [http://localhost:8000](http://localhost:8000). You can test it by navigating to [http://localhost:8000/api/ping](http://localhost:8000/api/ping) or [http://localhost:8000/docs](http://localhost:8000/docs) for the Swagger UI.

3.  **Stop the Application:**
    To stop and remove the containers, networks, and volumes created by `docker-compose up`, press `Ctrl+C` in the terminal where Docker Compose is running, and then run:
    ```bash
    docker-compose down
    ```
    If you ran `docker-compose up -d` (detached mode), you only need to run `docker-compose down`.

## Development without Docker

For individual development of the frontend or backend, refer to the `README.md` files in their respective directories:
-   [frontend/README.md](./frontend/README.md)
-   [backend/README.md](./backend/README.md)

These provide instructions for setting up development environments, installing dependencies, and running the applications natively.
