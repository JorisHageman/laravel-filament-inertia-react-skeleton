# Laravel Filament Inertia React Skeleton

This project is a pre-configured skeleton application that combines Laravel, Filament Admin Panel, Inertia.js and React to provide a comprehensive starting point for web application development.

## Features

- **Laravel 12.x** - Latest version of Laravel framework
- **Filament 3.x** - Admin panel toolkit for Laravel
- **Inertia.js** - Server-side rendering without API boilerplate
- **React 19** - Front-end library for building user interfaces
- **TypeScript** - Type safety for your JavaScript code
- **Docker** - Development environment using Laravel Sail
- **TailwindCSS 4** - Utility-first CSS framework

## Requirements

- PHP 8.2+
- Node.js
- Composer
- Docker & Docker Compose (for Sail)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/laravel-filament-inertia-react-skeleton.git
   cd laravel-filament-inertia-react-skeleton
   ```

2. Install PHP dependencies:
   ```bash
   composer install
   ```

3. Create environment file:
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Install JavaScript dependencies:
   ```bash
   npm install
   # or if using pnpm
   pnpm install
   ```

5. Start the development environment:
   ```bash
   # Using Laravel Sail (Docker)
   ./vendor/bin/sail up
   
   # Or using the composer script
   composer dev
   ```

## Usage

### Development

```bash
# Start all services (Laravel server, queue worker, logs, and Vite)
composer dev

# Start with SSR enabled
composer dev:ssr

# Run only Vite dev server
npm run dev
```

### Building for Production

```bash
# Build frontend assets
npm run build

# Build with SSR support
npm run build:ssr
```

### Code Quality

```bash
# Format code with Prettier
npm run format

# Check formatting
npm run format:check

# Lint JavaScript/TypeScript
npm run lint

# Type checking
npm run types

# Run tests
composer test
```

## Docker

This project uses Laravel Sail for Docker integration. The Docker setup includes:

- PHP 8.4 container
- MariaDB 10.6 database
- Node.js container for frontend development

You can start the Docker environment with:

```bash
./vendor/bin/sail up
```

## Project Structure

The project follows the standard Laravel structure with some additions:

- `/app` - Laravel application code
- `/resources/js` - React components and frontend code
- `/resources/css` - CSS files including Tailwind CSS
- `/public` - Compiled assets and static files

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
