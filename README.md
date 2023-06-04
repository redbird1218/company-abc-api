### Installation

`composer install`

copy the `.env.example` file to `.env` and supply the URL of your backend:

```
APP_URL=http://localhost:8000
FRONTEND_URL=http://localhost:3000
```

After defining the appropriate environment variables, you may serve the Laravel application using the `serve` Artisan command:

```bash
# Serve the application...
php artisan serve

#run the migration
php artisan migrate
```

## Or using Docker

> Make sure [Docker Desktop](https://www.docker.com/products/docker-desktop/) is installed and running

1. `mv .env.example .env`

2. `composer install`

3. `./vendor/bin/sail up`

4. `open Docker Desktop`

5. `open sail terminal`

6. `php artisan key:generate`

7. `php artisan migrate`

8. `visit http://localhost/`
