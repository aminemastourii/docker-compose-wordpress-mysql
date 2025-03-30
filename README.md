# WordPress with MySQL using Docker Compose

This project sets up a WordPress instance along with a MySQL database using Docker Compose. It is a quick and easy way to get a local WordPress environment running.

## Prerequisites

- **Docker**: Make sure Docker is installed on your machine. You can download Docker from [here](https://www.docker.com/get-started).
- **Docker Compose**: This is used to define and manage multi-container Docker applications. Docker Compose is typically included with Docker Desktop. If you need to install it separately, you can find instructions [here](https://docs.docker.com/compose/install/).

## Installation Steps

1. Clone this repository to your local machine:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Ensure Docker and Docker Compose are running on your machine.

3. Start the WordPress and MySQL containers by running:
   ```bash
   docker-compose up -d
   ```
   This will start the services in **detached mode** (running in the background).

4. Check if the containers are running:
   ```bash
   docker-compose ps
   ```

5. Open your browser and visit:
   ```
   http://localhost:8080
   ```
   This will open the WordPress installation page where you can set up your website.

## Stopping the Services

To stop and remove the containers, run:
```bash
docker-compose down
```
This will **stop** the services and remove the containers, but your data will persist if volumes are configured.

## Notes

- The default MySQL credentials are:
  - **Username:** `wpuser`
  - **Password:** `wppassword`
  - **Database Name:** `wordpress`