# HARSAC Website

This is an ASP.NET Core MVC application for the Haryana Space Applications Centre (HARSAC).

## Prerequisites

- [.NET 9.0 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
- [Docker](https://docs.docker.com/get-docker/) (optional, for containerization)

## Getting Started

### 1. Clone the Repository

If you haven't already, clone the repository to your local machine:

```bash
git clone <repository-url>
cd HarsacWebsite
```

## Running Locally (Windows/Linux/macOS)

To run the application directly using the .NET CLI:

```bash
dotnet run
```

The application will be available at `http://localhost:5270`.

## Running with Docker (Recommended for Linux)

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

## Linux Quick Start Guide

If you are on a fresh Linux machine (e.g., Ubuntu), follow these steps:

1.  **Install Docker:**
    ```bash
    curl -fsSL https://get.docker.com -o get-docker.sh
    sudo sh get-docker.sh
    sudo usermod -aG docker $USER
    # Log out and back in for group changes to take effect
    ```

2.  **Get the Code:**
    ```bash
    git clone <your-repo-url>
    cd HarsacWebsite
    ```

3.  **Run with Docker:**
    ```bash
    docker build -t harsac-website .
    docker run -d -p 8080:8080 --name harsac-app harsac-website
    ```
