# Docker Compose Guide

## What Does the Services Block Do?

The `services:` block defines the containers that will be used in the application. In this mission, it contains two services: `database` and `app`. The database service uses MariaDB, while the app service uses Nextcloud.

## How Does Nextcloud Find the Database?

Nextcloud finds the database through the `MYSQL_HOST=database` environment variable. The value `database` matches the service name defined in the Docker Compose file. Docker Compose allows the containers to communicate using their service names within the same network.

## Difference Between docker run and docker-compose up -d

The `docker run` command is used to create and start an individual container with manually specified settings. In contrast, `docker-compose up -d` reads the `docker-compose.yml` file and starts the services defined in it. Docker Compose makes it easier to deploy and manage multiple related containers using a single command.

## Conclusion

Docker Compose helps cloud engineers manage multi-container applications more efficiently. It also supports Infrastructure as Code (IaC) by allowing deployment settings to be written, saved, reused, and documented in a configuration file.
