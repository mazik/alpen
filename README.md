<h1 align="center"><img src="https://user-images.githubusercontent.com/8946603/184360010-a3b2280f-d9d0-4b0e-b960-2a5bcf53d061.svg" alt="alpen"></h1>

## Introduction
Alpen is a lightweight Docker image for building an Nginx server with PHP. The goal is to use the latest alpine Docker image to make Nginx and PHP without hardcoding the version number on the `docker-compose.yml` to ensure we always have the newest version in place.

## Why?
I couldn't find a simple Docker image that's easy to understand and doesn't add any extension to quickly spin up an Nginx server with the latest version of PHP.

> It doesn't come with any PHP extension installed to keep it simple. So, it won't work when connecting with MySQL or any other database engines.

## Installation
1. Clone the repository `https://github.com/mazik/alpen`
2. Spin up Docker container `docker compose up -d`
3. Place your PHP files under the `www` directory
4. Visit `http://localhost:80`

## License
Alpen is open-sourced software licensed under the [MIT license](LICENSE.md).
