# Caddy Reverse Proxy

The Caddy server reverse proxy to endpoints.

## Getting Started

Prerequisites
Before you begin, ensure you have the following installed on your machine:

Docker: Download and install Docker from the [official Docker website](https://www.docker.com/products/docker-desktop/).

## Running the Project

Clone the Repository: Download or clone the project files to your local machine.

Open the Caddyfile and change the `https://your-endpoint.net` with the address to forward the local address to.

Open a Terminal: Navigate to the directory where the docker-compose.yml file is located.

Start the Caddy Server: Run the following command to start the reverse proxy:

```
 docker-compose up -d
```

Verify the Startup: You should see output similar to the following, indicating that the Caddy container has started successfully:

```
Container caddy-caddy-1  Started
```

This will start the reverse proxy.

## Accessing the Service

The Caddy server will be available at http://localhost on port 80. If you've configured other ports in your docker-compose.yml, you can access them accordingly.

## Stopping the Service

To stop the Caddy server, you can run:

```
Container caddy-caddy-1  Started
```

This will stop and remove the containers defined in your docker-compose.yml file.

## Configuration

If you need to adjust the configuration (such as changing endpoints or adding middleware), edit the Caddyfile located in the project directory. After making changes, restart the Caddy service with:

```
docker-compose restart
```

Feel free to adjust any sections according to your needs!
