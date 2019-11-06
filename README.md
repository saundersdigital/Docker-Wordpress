# WordPress Docker Container

WordPress container with Nginx 1.16.1, PHP-FPM 7.3 & MariaDB 10.4.8.

_WordPress version currently installed:_ **5.2.4**

## Installation

Open a terminal and `cd` to the folder in which `docker-compose.yml` is saved and run:

```
docker-compose up -d
```

This creates two new folders next to your docker-compose.yml file.

* `db_data` - used to store and restore database dumps
* `code` - here you copy your existing WordPress code

The containers are now built and running. You should be able to access the WordPress installation with the configured IP in the browser address. By default it is `http://127.0.0.1`.

## Usage

### Starting containers

You can start the containers with the `up` command in daemon mode (by adding `-d` as an argument) or by using the `start` command:

```
docker-compose start
```

### Stopping containers

```
docker-compose stop
```

### Removing containers

To stop and remove all the containers use the`down` command:

```
docker-compose down
```
