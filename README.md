
# WordPress Docker Container

Lightweight WordPress container with Nginx 1.24 & PHP-FPM 8.3 based on Alpine Linux.

_WordPress version currently installed:_ **6.4.3**

* Used in production for many sites, making it stable, tested and up-to-date
* Optimized for 100 concurrent users
* Optimized to only use resources when there's traffic (by using PHP-FPM's ondemand PM)
* Works with Amazon Cloudfront or CloudFlare as SSL terminator and CDN
* Multi-platform, supporting AMD4, ARMv6, ARMv7, ARM64
* Built on the lightweight Alpine Linux distribution
* Small Docker image size (+/-90MB)
* Uses PHP 8.3 for the best performance, low cpu usage & memory footprint
* Can safely be updated without losing data
* Fully configurable because wp-config.php uses the environment variables you can pass as an argument to the container

![nginx 1.24](https://img.shields.io/badge/nginx-1.24-brightgreen.svg)
![php 8.3](https://img.shields.io/badge/php-8.3-brightgreen.svg)
![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)

## Usage
See [docker-compose.dev.yml](https://github.com/increact/docker-wordpress/blob/master/docker-compose.dev.yml) how to use it in your own environment.

    docker-compose up

### WP-CLI

This image includes [wp-cli](https://wp-cli.org/) which can be used like this:

    docker exec <your container name> /usr/local/bin/wp --path=/usr/src/wordpress <your command>

# thing to update being use
Dockerfile wordpress version
config/msmtprc domain name
.env
docker-compose service information
BE REINDED that config file is cpy into the docker during start up, any change require to re build the docker image

## forked from 

* https://github.com/TrafeX/docker-wordpress
