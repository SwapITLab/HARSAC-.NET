# HARSAC Website

This is an ASP.NET Core MVC application for the Haryana Space Applications Centre (HARSAC).

## Prerequisites

- .NET 9.0 SDK
- Docker (optional, for containerization)

## Running Locally

To run the application locally:

```bash
dotnet run
```

The application will be available at `http://localhost:5270`.

## Running with Docker

To run the application using Docker, ensure Docker is installed and running on your machine.

### 1. Build the Docker Image

Run the following command in the project root directory:

```bash
docker build -t harsac-website .
```

### 2. Run the Docker Container

Run the container and map port 8080 to a local port (e.g., 8080):

```bash
docker run -d -p 8080:8080 --name harsac-app harsac-website
```

The application will be accessible at `http://localhost:8080`.

### 3. Stop and Remove the Container

To stop the container:

```bash
docker stop harsac-app
```

To remove the container:

```bash
docker rm harsac-app
```
