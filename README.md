# WebServer

Version 1 LNMP

### Architecture

![architecture][1]

The whole app is divided into three Containers:

1. Nginx is running in `Nginx` Container, which handles requests and makes responses.
2. PHP or PHP-FPM is put in `PHP-FPM` Container, it retrieves php scripts from host, interprets, executes then responses to Nginx. If necessary, it will connect to `MySQL` as well.
3. MySQL lies in `MySQL` Container,
 
Reference: https://github.com/micooz/docker-lnmp.git

[1]: architecture.png
