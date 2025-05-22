# Backend Application (FastAPI)

This is the backend application built with FastAPI and Python.

## Development

### Prerequisites
- Python (version 3.7 or higher recommended)
- pip

### Setting up the Environment and Installing Dependencies
1.  **Create a virtual environment:**
    Navigate to the `backend` directory and run:
    ```bash
    python -m venv venv
    ```
2.  **Activate the virtual environment:**
    -   On macOS and Linux:
        ```bash
        source venv/bin/activate
        ```
    -   On Windows:
        ```bash
        .\venv\Scripts\activate
        ```
3.  **Install dependencies:**
    With the virtual environment activated, install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Development Server
To start the FastAPI development server, run the following command from the `backend` directory:
```bash
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```
The API will be accessible at [http://localhost:8000](http://localhost:8000). The server will automatically reload when code changes are detected.

## Docker
This application can also be built and run using Docker. Refer to the main `README.md` in the root directory for instructions on using Docker Compose.
