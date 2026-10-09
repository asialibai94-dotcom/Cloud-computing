# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is an application structure that separates a system into two main parts: the Web/Application Tier and the Database Tier. These two tiers communicate with each other to provide services to users and manage data efficiently.

## The Web/Application Tier

The Web/Application Tier is responsible for displaying the user interface and handling user requests. In this mission, Nextcloud serves as the web application that allows users to access and manage their files through a web browser.

## The Database Tier

The Database Tier stores and manages persistent data, such as user accounts, credentials, and file metadata. In this mission, MariaDB serves as the database that stores the information required by Nextcloud.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. It also allows each service to be updated or scaled independently. If one container encounters a problem, separating the services can make it easier to identify and resolve the issue.

## Architecture Components

- **Web/Application Tier:** Nextcloud
- **Database Tier:** MariaDB
- **Communication:** Docker Compose connects the application to the database using the `MYSQL_HOST=database` environment variable.
