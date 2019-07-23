# LAMP

A basic LAMP environment for docker.

### Images

- php:5.5.25-apache
- mysql:5.7.12
- adminer

### Installation

Install the required dependencies.

```sh
$ git clone https://github.com/robertosegura/docker-lamp.git
```

```sh
$ echo "<?php phpinfo(); ?>" >> code/index.php
```

### DB Connection

Update the correct database, root password.

```yaml
environment:
  - MYSQL_ROOT_PASSWORD=root
  - MYSQL_DATABASE=db
```

### Import SQL backup

Place your .sql to mysql/dump.sql
