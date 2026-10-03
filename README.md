# Laravel Example App

A starter web application built with Laravel 10. It currently contains Laravel's default welcome page, a sample `User` model and factory, database migrations, and a Vite setup for frontend assets. Use it as a foundation for building a Laravel application.

## About Laravel

[Laravel](https://laravel.com) is an open-source PHP framework for building web applications. It provides tools for common tasks such as URL routing, database access and migrations, authentication, and rendering views. This project uses Laravel 10 as its application framework.

## Requirements

- PHP 8.1 or later
- Composer
- Node.js and npm
- A database configured in your environment if you plan to run migrations

## Setup

```bash
composer install
cp .env.example .env
php artisan key:generate
npm install
npm run build
```

Configure the database settings in `.env`, then run migrations if needed:

```bash
php artisan migrate
```

Start the local server:

```bash
php artisan serve
```

For frontend development with Vite, run `npm run dev` in a separate terminal.
