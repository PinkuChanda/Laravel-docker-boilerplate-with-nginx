# Laravel Docker Boilerplate with Nginx
Docker setup for Laravel with Nginx and MySQL. Quickly spin up a Laravel environment with optimized configurations for PHP and Nginx. 

This boilerplate provides a ready-to-use Docker setup for Laravel, utilizing Nginx, PHP, MySQL, Composer, Artisan, Node (NPM), and Mailpit for a complete development environment.

## Prerequisites

- Docker & Docker Compose installed

## Setup Guide

**Clone the Repository**
   ```
   git clone <repo-url>
   cd <repo-directory>
   ```

**Configure Environment**

Ensure you have a `.env` file in your Laravel `src` directory with the appropriate configuration. Here are the recommended settings for database and mail service:

```
DB_HOST=mysql
DB_DATABASE=database_name
DB_USERNAME=database_user_name
DB_PASSWORD=database_password
MAIL_HOST=mailpit
MAIL_PORT=1025
```
**Start Docker Containers**

To start all services, run:

```
docker compose up -d --build
```

* **Nginx:** http://localhost
* **Mailpit Interface:** http://localhost:8025