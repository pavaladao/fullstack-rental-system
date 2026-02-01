# Full Stack Development Course Project

A full-stack application built as part of a university full-stack development course, showcasing backend APIs and frontend integration.

## Overview

This repository contains multiple backend APIs and database configurations implemented as part of a full-stack development curriculum. The project demonstrates RESTful API design, Docker usage, and basic integration between services.

## Features

- **RESTful APIs**: Backend services for different domain entities (e.g., person, car, rental, client)
- **Database with Docker**: MySQL database configured with Docker for local development
- **Modular Architecture**: Separate API modules that can be individually deployed and tested

## Technologies Used

- **Python**: Main backend language
- **Flask / REST Framework**: For building REST APIs
- **MySQL**: Relational database for data persistence
- **Docker**: Containerized database environment
- **HTML**: Static pages or simple frontend components (if present)

## Project Structure

```plaintext
projeto_fullstack/
├── pessoa_api/            # Person API microservice
├── carro_api/             # Car API microservice
├── aluguel_api/           # Rental API microservice
├── client_api/            # Client API microservice
├── mysql/                 # MySQL Docker configuration
└── README.md              # Project documentation
```

## Getting Started (Local Setup)

### Prerequisites

Make sure you have installed:

- Docker (to run the database)
- Python 3.x
- pip (Python package manager)

### Install Dependencies

1. Navigate to each API folder (for example `pessoa_api/`)
2. Install Python dependencies:

   ```bash
   pip install -r requirements.txt
   ```

### Run MySQL with Docker

From the `mysql/` directory:

```bash
docker compose up -d
```

This will start a MySQL database in a container that the backend services can connect to.

### Run Backend APIs

In each API folder, start the server:

```bash
python app.py
```

The APIs should be accessible locally (e.g., `http://localhost:PORT/...`) depending on your configuration.

## Usage

After setup, you can use tools like Postman or curl to make requests to individual API endpoints. Refer to each API's route definitions for available operations (GET, POST, PUT, DELETE).

## Testing

If there are test scripts, run them with:

```bash
pytest
```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve functionality, add documentation, or fix bugs.

## License

This project is part of an academic course and isn't licensed for commercial use. Feel free to explore and learn from the implementation.
