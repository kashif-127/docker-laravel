# Docker Images for Laravel builds
This repository contains a docker image for laravel builds. Php, fpm, mysql, redis installed.


## Installation

1. Install [docker](https://docs.docker.com/engine/installation/) and [docker-compose](https://docs.docker.com/compose/install/) ;

2. Copy `docker-compose.yml` file to your project root path, and edit it according to your needs ;

3. From your project directory, start up your application by running:

```sh
docker-compose up
```
4. If you want, you can run composer or artisan through docker. For instance:

```sh
docker-compose exec php composer install
docker-compose exec php php artisan migrate
docker-compose exec php $yourCommandHere
```


## Docker Images

These docker images are configured in `docker-compose.yml` file.
You can comment or uncomment some services according to your project.

* [`kashifz/php-fpm-laravel-mysql-redis:7.4`](https://hub.docker.com/r/toblerone/laravel-php/) (this docker image extends `php:7.4-fpm-alpine` to add some PHP extensions) ;
* `mysql:5.7` ;
* `redis:4.0-alpine` ;

## Contributing

Contributions are welcome!
Leave an issue on Github, or create a Pull Request.


## Licence

This work is under [MIT](LICENCE) licence.
