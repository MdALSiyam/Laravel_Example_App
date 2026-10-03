# Laravel Example App

A starter web application built with Laravel 10. It currently contains Laravel's default welcome page, a sample `User` model and factory, database migrations, and a Vite setup for frontend assets. Use it as a foundation for building a Laravel application.

## About Laravel

[Laravel](https://laravel.com) is an open-source PHP framework for building web applications. It provides tools for common tasks such as URL routing, database access and migrations, authentication, and rendering views. This project uses Laravel 10 as its application framework.

## Laravel Components in This Project

- `routes/web.php` defines website routes. The `/` route currently displays the default page in `resources/views/welcome.blade.php`.
- `routes/api.php` is where API routes can be defined.
- `app/Http/Controllers/` contains the base controller for handling application requests; no feature-specific controllers are implemented yet.
- `app/Models/User.php` is the Eloquent model for users.
- `database/migrations/` defines the database tables. `database/factories/` and `database/seeders/` support generating and inserting sample data.
- `resources/views/` contains Blade templates. `resources/css/`, `resources/js/`, and `vite.config.js` provide the frontend asset setup with Vite.
- `config/` contains Laravel configuration, while `bootstrap/app.php` initializes the application.
- `public/index.php` is the web entry point, and `artisan` provides Laravel's command-line tools.
- `tests/` contains the application's feature and unit tests.

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
