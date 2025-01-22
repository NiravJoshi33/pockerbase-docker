# pockerbase-docker

Deploy PocketBase using Docker

## Overview

PocketBase is a lightweight, open-source backend solution that provides a real-time database and user authentication. This repository contains a Docker setup for easy deployment of PocketBase.

## Prerequisites

- Docker installed on your machine
- Docker Compose (optional, for easier management)

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yourusername/pockerbase-docker.git

cd pocketbase-docker
```

### Build the Docker Container

```bash
docker run -d -p 8090:8090 pocketbase
```

### Using Docker Compose

Alternatively, you can use Docker Compose for easier management:

```bash
docker-compose -f compose.pocketbase.yaml up --build -d
```

## Configuration

You can customize the environment variables in `compose.pocketbase.yaml`:

- `ENCRYPTION`: Set a secure encryption key for your application.

## Volumes

- `./pb_migrations`: Directory for database migrations.
- `./pb_hooks`: Directory for custom hooks.

## Accessing PocketBase

Once the container is running, you can access PocketBase at `http://localhost:8090`.

## Contributing

Feel free to submit issues or pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
