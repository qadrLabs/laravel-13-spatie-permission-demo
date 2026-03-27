# Laravel 13 Role-Based Access Control Demo

This project is a demonstration of implementing Role-Based Access Control (RBAC) in Laravel 13 using the [Spatie Laravel Permission](https://github.com/spatie/laravel-permission) package and Laravel's Middleware Attributes.

This repository is part of the tutorial: [Laravel 13: Role-Based Access Control with Spatie Permission and Middleware Attributes](https://qadrlabs.com/post/laravel-13-role-based-access-control-with-spatie-permission-and-middleware-attributes).

## Prerequisites

- PHP 8.3 or higher
- Composer
- Node.js & NPM
- SQLite (or your preferred database)

## Installation and Setup

Follow these steps to set up the project locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/qadrLabs/laravel-13-spatie-permission-demo.git
   cd laravel-13-spatie-permission-demo
   ```

2. **Install PHP dependencies:**
   ```bash
   composer install
   ```

3. **Install NPM dependencies:**
   ```bash
   npm install
   ```

4. **Environment Configuration:**
   Copy the example environment file and generate the application key.
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. **Database Migration and Seeding:**
   Run the migrations along with the seeders to set up default roles, permissions, and test users.
   ```bash
   php artisan migrate --seed
   ```

6. **Build Frontend Assets:**
   ```bash
   npm run build
   ```

7. **Run the Application:**
   ```bash
   php artisan serve
   ```

## Roles and Test Accounts

The following roles and permissions are configured by default:

- **Admin**: Has full access (all permissions).
- **Editor**: Can view, create, edit, and publish articles.
- **Viewer**: Can only view articles.

### Default Test Users

All users have the password: `password`

- **Admin**: `admin@example.com`
- **Editor**: `editor@example.com`
- **Viewer**: `viewer@example.com`

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
