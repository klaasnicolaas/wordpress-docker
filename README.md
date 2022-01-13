<!--
*** To avoid retyping too much info. Do a search and replace for the following:
*** github_username, repo_name
-->

# 🌐 Wordpress docker - Template
<!-- PROJECT SHIELDS -->
![Project Maintenance][maintenance-shield]
[![License][license-shield]](LICENSE.md)

[![GitHub Activity][commits-shield]][commits]
[![GitHub Last Commit][last-commit-shield]][commits]
[![Contributors][contributors-shield]][contributors-url]

[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## About

This is a template repository for running Wordpress within a Docker environment. With the approach that it is easy to set up and you can run many wordpress environments on a single host.

## Get started

How to start with this Laravel Docker template:

1. Clone the repository
2. Create a `.env` file

```bash
cp .env.example .env
```

3. Inside the `.env` file give the following variables a value
    - `APP_NAME`
    - `APP_PORT`
    - `MYSQL_HOST`
    - `MYSQL_PORT`
    - `MYSQL_ROOT_PASSWORD`
    - `MYSQL_USERNAME`
    - `MYSQL_PASSWORD`

### Ports (optional)

By default port **8000** is set for Wordpress and **3306** for MySQL, if you prefer to use other ports you can change this in the created `.env` file.

### Volumes (optional)

If you want to access the persistent data from the containers, you just have to uncomment the volumes in the [docker-compose.yml](docker-compose.yml) file.

## Run

When you have done the getting started part, it's time to start the docker containers.

```bash
docker-compose up -d
```

## Contributing

Would you like to contribute to the development of this project? Then read the prepared [contribution guidelines](CONTRIBUTING.md) and go ahead!

Thank you for being involved! :heart_eyes:

## License

MIT License

Copyright (c) 2021-2022 Klaas Schoute

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

<!-- MARKDOWN LINKS & IMAGES -->
[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg?style=for-the-badge
[contributors-shield]: https://img.shields.io/github/contributors/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[contributors-url]: https://github.com/klaasnicolaas/wordpress-docker/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[forks-url]: https://github.com/klaasnicolaas/wordpress-docker/network/members
[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[stars-url]: https://github.com/klaasnicolaas/wordpress-docker/stargazers
[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[issues-url]: https://github.com/klaasnicolaas/wordpress-docker/issues
[license-shield]: https://img.shields.io/github/license/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/wordpress-docker.svg?style=for-the-badge
[commits]: https://github.com/klaasnicolaas/wordpress-docker/commits/master
[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/wordpress-docker.svg?style=for-the-badge