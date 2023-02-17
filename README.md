# Laravel Boilerplate

Requirements:
- Docker Desktop

Installation:
- Clone this repository.
- cd into it
- Install dependencies with the following:
```
docker run --rm \
   -u "$(id -u):$(id -g)" \
   -v "$(pwd):/var/www/html" \
   -w /var/www/html \
   laravelsail/php82-composer:latest \
   composer install --ignore-platform-reqs
```
- copy .env.example to .env
- run `sail up -d`
- `sail npm install`
- `sail npm run dev` to generate vite manifest
- run migrations with `sail artisan migrate`
- visit: http://localhost:80

Stack:
- Laravel
- MySQL
- Blade
- AlpineJS
- TailwindJS
