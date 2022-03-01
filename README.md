# php70-nginx-postgres

Docker for development environment using Laravel

- Laravel 5.2
- PHP7.0-FPM
- NGINX
- Postgres Database (max version 9.6, 10 up have problem with SCRAM authentication in apple m1 docker)

# config

- copy and configure `.env` from `.env.example`
- copy and configure `/nginx/web.conf` from `/nginx/web.conf`
- run `sudo docker-compose build app` to create app image from dockerfile
- run `sudo docker-compose up -d`

# Laravel

- use `sudo docker exec [container_name] composer [composer command]` to run composer command.
- use `sudo docker exec [container_name] php artisan [artisan command]` to run artisan command.

## Fajar Pratama (omclabs@gmail.com)
