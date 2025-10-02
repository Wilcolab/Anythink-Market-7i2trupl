# Express Server Project

This project is a simple Express server that listens on port 8001. It is set up to use Nodemon for automatic code reloading during development.

## Project Structure

```
express-server
├── src
│   └── index.js          # Entry point of the application
├── package.json          # Configuration file for npm
├── yarn.lock             # Yarn lock file for dependency versions
├── Dockerfile            # Dockerfile to build the application image
├── .gitignore            # Files and directories to ignore by Git
├── nodemon.json          # Configuration settings for Nodemon
└── README.md             # Project documentation
```

## Getting Started

### Prerequisites

- Node.js and Yarn should be installed on your machine.

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd express-server
   ```

2. Install the dependencies:
   ```
   yarn install
   ```

### Running the Server

To start the server with automatic reloading, use the following command:

```
yarn start
```

The server will be running on [http://localhost:8001](http://localhost:8001).

### Docker

To build and run the application using Docker, use the following commands:

1. Build the Docker image:
   ```
   docker build -t express-server .
   ```

2. Run the Docker container:
   ```
   docker run -p 8001:8001 express-server
   ```

### License

This project is licensed under the MIT License.