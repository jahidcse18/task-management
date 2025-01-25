# Task Management API

A simple Task Management API built with Laravel 11. This API allows users to create, view, mark tasks as completed, and delete tasks.

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Setup .env](#setup-env)
- [Running the Project Locally](#running-the-project-locally)
- [Testing the API](#testing-the-api)
- [Sample .env.example](#sample-envexample)
- [License](#license)

## Requirements

- PHP 8.1 or higher
- Composer
- MySQL or another database of your choice
- Laravel 11

## Installation

Follow these steps to set up and run the project locally:

1. Clone the repository:

    ```bash
    git clone https://github.com/jahidcse18/task-management.git
    ```

2. Navigate to the project directory:

    ```bash
    cd task-management-api
    ```

3. Install the dependencies using Composer:

    ```bash
    composer install
    ```

4. Copy the `.env.example` file to `.env`:

    ```bash
    cp .env.example .env
    ```

5. Generate the application key:

    ```bash
    php artisan key:generate
    ```

6. Set up the database configuration in your `.env` file:
    - Edit `.env` and set the correct database credentials (DB_HOST, DB_DATABASE, DB_USERNAME, DB_PASSWORD).

## Setup .env

Create a `.env` file by copying `.env.example` and configure your database connection.

### Sample `.env.example`

```env
APP_NAME=Laravel
APP_ENV=local
APP_KEY=base64:randomgeneratedkeyhere
APP_DEBUG=true
APP_URL=http://localhost

LOG_CHANNEL=stack

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=task_management
DB_USERNAME=root
DB_PASSWORD=

BROADCAST_DRIVER=log
CACHE_DRIVER=file
QUEUE_CONNECTION=sync
SESSION_DRIVER=file
SESSION_LIFETIME=120

# Uncomment and set if you are using a mail service
# MAIL_MAILER=smtp
# MAIL_HOST=smtp.mailtrap.io
# MAIL_PORT=2525
# MAIL_USERNAME=null
# MAIL_PASSWORD=null
# MAIL_ENCRYPTION=null
# MAIL_FROM_ADDRESS="hello@example.com"
# MAIL_FROM_NAME="${APP_NAME}"

# Uncomment and set if you are using API authentication
# SANCTUM_STATEFUL_DOMAINS=localhost
