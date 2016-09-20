# WebServer

Version 1 LNMP (Linux, Nginx, PHP7, Mysql)
Nginx and Mysql use the latest official image.

### Architecture

![architecture][1]

The whole app is divided into three Containers:

1. Nginx is running in `Nginx` Container, which handles requests and makes responses.
2. PHP or PHP-FPM is put in `PHP-FPM` Container, it retrieves php scripts from host, interprets, executes then responses to Nginx. If necessary, it will connect to `MySQL` as well.
3. MySQL lies in `MySQL` Container,
 
Reference: https://github.com/micooz/docker-lnmp.git

[1]: architecture.png

### Build and Run
At first, you should have had Docker and Docker Compose installed.

Without building images one by one, you can make use of docker-compose and simply issue:

	$ sudo docker-compose up

For more operations to containers, please refer to:

	$ sudo docker-compose --help

### License

MIT
