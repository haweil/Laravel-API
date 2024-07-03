# Laravel API

This project is a simple Laravel API that demonstrates CRUD operations for managing authors and books using the repository pattern. It includes resource collections, email functionality, task scheduling, and authentication with protected routes.

## Features

- **CRUD API**: Perform Create, Read, Update, and Delete operations for authors and books.
- **Repository Pattern**: Implements the repository pattern for better code organization and separation of concerns.
- **Resource Collections**: Use resource collections to transform data for API responses.
- **Email Functionality**: Send emails using Laravel's built-in email capabilities.
- **Task Scheduling**: Schedule tasks to run at specific intervals using Laravel's task scheduler.
- **Authentication**: User registration and login with token-based authentication to protect routes and API endpoints.
## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/laravel-api.git
2. **Navigate to the project directory:**
    ```bash
      cd laravel-api

3. Install dependencies:
   ```bash
   composer install
   npm install

4. Copy the .env.example file to .env and configure your environment variables:
   ```bash
      cp .env.example .env
    

5. Run database migrations and seeders:
   ```bash
      php artisan migrate --seed
## Usage

### Start the Laravel Development Server:
```bash
php artisan serve
```
### Authentication Endpoints:
- Register: POST /api/register
- Login: POST /api/login
- Logout: POST /api/logout (requires token)

### API Endpoints (Protected):
## Authors :
- Create an author: POST /api/authors (requires token)
- Read authors: GET /api/authors (requires token)
- Read a single author: GET /api/authors/{id} (requires token)
- Update an author: PUT /api/authors/{id} (requires token)
- Delete an author: DELETE /api/authors/{id} (requires token)
## Books:
- Create a book: POST /api/books (requires token)
- Read books: GET /api/books (requires token)
- Read a single book: GET /api/books/{id} (requires token)
- Update a book: PUT /api/books/{id} (requires token)
- Delete a book: DELETE /api/books/{id} (requires token)

