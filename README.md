# symfony6-docker-template
Symfony 6 only with Docker containers. Ready to use.


## Run Locally

Clone the project

```bash
  git@github.com:francoiscoche/symfony6-docker-template.git
```

Run the docker-compose

```bash
  docker-compose build
  docker-compose up -d
```

Log into the PHP container

```bash
  docker exec -it php8 bash
```

Create your Symfony application and launch the internal server

```bash
  symfony new new-project --webapp
  cd new-project
  symfony serve -d
```


*The application is available at http://127.0.0.1:9000*

Modify the .env to access to the database:

```yaml
    DATABASE_URL="mysql://root:root@db:3306/db_name"
```

## Ready to use with

This docker-compose provides you :

- PHP-8
    - Composer
    - Symfony CLI
    - and some other php extentions
    - nodejs, npm, yarn
- mysql


## Requirements

- Docker
- Docker-compose


## Author

Adapted by [@francoiscoche](https://github.com/francoiscoche)
Thanks to [@yoanbernabeu](https://github.com/yoanbernabeu)
