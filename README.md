# How it Works

Docker builds an image containing the application in src/ and all of its dependencies by using the Dockerfile contained in this repository.

The Dockerfile tells docker to use the [official PHP Docker image](https://hub.docker.com/_/php/) as the parent image.

The PHP image then uses the [official Debian Jessie Docker image](https://hub.docker.com/_/debian/) as its parent image.

Debian then uses the [scratch image](https://hub.docker.com/_/scratch/) as its base image.


# Setup

 - Ensure you have Docker installed
 - `git clone` this repository
 - `sudo docker build -t docker-php-helloworld .` 
 - `sudo docker run -p 80:80 docker-php-helloworld`

