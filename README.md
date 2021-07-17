# php70-nginx-postgres

Docker for development environment using Laravel

- Laravel 5.2
- PHP7.0-FPM
- NGINX
- Postgres Database

# config

- copy and configure `.env` from `.env.example`
- copy and configure `/nginx/web.conf` from `/nginx/web.conf`
- run `sudo docker-compose build app` to create app image from dockerfile
- run `sudo docker-compose up -d` or run `sudo docker-compose up -d --scale app=[xx]`

# Laravel

- use `sudo docker exec [container_name] composer [composer command]` to run composer command.
- use `sudo docker exec [container_name] php artisan [artisan command]` to run artisan command.

# Postgres DB

- use `psql -U [POSTGRES_USER] -W [POSTGRESS_PASSWORD] -h 127.0.0.1 -p 55432` to connect to DB from host.
- use `psql -U [POSTGRES_USER] -W [POSTGRESS_PASSWORD] -h 127.0.0.1 -p 55432 -f [SQL FILE PATH]` to import sql file to DB from host.
- use port 55432 in case you already have postgres sql in host machine.

## Fajar Pratama (omclabs@gmail.com)
