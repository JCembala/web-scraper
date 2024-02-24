# Web Scraper

This is a web scraper application built with Ruby and JavaScript. It uses PostgreSQL for the database and Redis for caching.

## Prerequisites

- Ruby 3.2.2

## Setup

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Copy the `.env.template` file and rename the copy to `.env`.
4. Update the `.env` file with your actual credentials and settings.
5. You can run `asdf install` to install the Ruby version defined in the `.tool-versions` file.

## Local Development
In local development, you can use Docker to run the PostgreSQL and Redis services.

First, run the following command to start the PostgreSQL and Redis services:

```bash
docker-compose up
```
This command will start the PostgreSQL and Redis services as defined in the `docker-compose.yml` file.  Please ensure that the `.env` file is correctly set up with your database credentials and other environment variables.

Next, run the following command to create the database and run the migrations:

```bash
rails db:create db:migrate
```

After the database is set up, you can start the Rails server with the following command:

```bash
rails s
```