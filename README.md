
# Python Server

This project contains a FastAPI server implemented in Python. It provides two routes for managing a task list.

# Node Server

This project contains a Node.js Express server. It provides two routes for managing a task list, similar to the Python FastAPI server.

## Project Structure

The project has the following files and directories:

- `express-server/src/index.js`: This file contains the implementation of the Express server with two routes. It handles adding a task to a list and retrieving the list.
- `express-server/package.json`: Lists dependencies required for the Express server.
- `express-server/Dockerfile`: Used to build a Docker image for the Express server. It specifies the base image, copies the source code, installs dependencies, and sets the command to run the server.
- `express-server/nodemon.json`: Configuration for nodemon to enable hot-reloading during development.
- `express-server/yarn.lock`: Dependency lock file for Yarn.

## Getting Started

To run the Express server using Docker, follow these steps:

- Build and start the Docker containers by running the following command:

  ```shell
  docker compose up
  ```

  This command will build the Docker image for the Express server and start the containers defined in the `docker-compose.yml` file.

- The Express server should now be running. You can access it at port `8001`.

## API Routes

The Express server provides the following API routes:

- `POST /tasks`: Adds a task to the task list. The request body should contain the task details as `{ "text": "your task" }`.
- `GET /tasks`: Retrieves the task list.


## Project Structure

The project has the following files and directories:

- `python-server/src/main.py`: This file contains the implementation of the FastAPI server with two routes. It handles adding a task to a list and retrieving the list.

- `python-server/src/__init__.py`: This file is an empty file that marks the `src` directory as a Python package.

- `python-server/requirements.txt`: This file lists the dependencies required for the FastAPI server and other dependencies.

- `python-server/Dockerfile`: This file is used to build a Docker image for the FastAPI server. It specifies the base image, copies the source code into the image, installs the dependencies, and sets the command to run the server.

- `docker-compose.yml`: This file is used to define and run multi-container Docker applications. It specifies the services to run, their configurations, and any dependencies between them.

## Getting Started

To run the FastAPI server using Docker, follow these steps:

- Build and start the Docker containers by running the following command:

  ```shell
  docker compose up
  ```

  This command will build the Docker image for the FastAPI server and start the containers defined in the `docker-compose.yml` file.

- The FastAPI server should now be running. You can access at port `8000`.

## API Routes

The FastAPI server provides the following API routes:

- `POST /tasks`: Adds a task to the task list. The request body should contain the task details.

- `GET /tasks`: Retrieves the task list.
