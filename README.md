# nextcloud-docker-postgresql-redis

All in one Nextcloud Docker build, using [NGINX](https://www.nginx.com/), [PostgreSQL](https://www.postgresql.org/) and [Redis](https://redis.io/). SSL certificate management with Certbot and [let's encrypt](https://letsencrypt.org/).

Current stack versions

- php 8.2 Alpine based (php:8.2-fpm-alpine)
- Nextcloud 26.0.0 
- PostgreSQL 14
- Redis (latest Alpine image)


# Getting started

Create your own configuration from the provided `.env.dist`

```bash
cp .env.dist .env
```

Then simply build all needed containers using compose

```bash
docker compose up --build
```

That's all folks, now you can browse [http://cloud.example.localhost:8888/](http://cloud.example.localhost:8888/) or [http://localhost:8888/](http://localhost:8888/) to setup and try Nextcloud with this stack.

Read this article for more info and learn how to run production ready Nextcloud instance using this project [https://dev.to/nicolasbonnici/dockerize-nextcloud-with-postgre-and-redis-16jl](https://dev.to/nicolasbonnici/dockerize-nextcloud-with-postgre-and-redis-16jl)

Feel free to use, fork, contribute and maintain this project.