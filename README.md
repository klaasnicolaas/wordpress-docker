# 🌐 Wordpress docker - Template
<!-- PROJECT SHIELDS -->
![Project Maintenance][maintenance-shield]
[![License][license-shield]](LICENSE)

[![GitHub Activity][commits-shield]][commits]
[![GitHub Last Commit][last-commit-shield]][commits]
[![Contributors][contributors-shield]][contributors-url]

[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## About

This is a template repository for running WordPress within a Docker environment. The goal is to make setup easy and allow you to run multiple WordPress environments on a single host.

## 🧪 Project structure

```
wordpress-docker/
├── docker-compose.yml
├── .env.example
├── config/
│   └── php/
│       └── uploads.ini
├── website/
└── README.md
```

## Get started

How to start with this WordPress Docker template:

1. Clone the repository
2. Create a `.env` file

```bash
cp .env.example .env
```

3. In the `.env` file, set the following variables:

- `APP_NAME` — Name of the project (used in container names)
- `APP_PORT` — Port to access WordPress (e.g. 8000)
- `MYSQL_HOST` — Usually `mysql`
- `MYSQL_PORT` — Usually `3306`
- `MYSQL_ROOT_PASSWORD` — Root password for MySQL
- `MYSQL_USER` — Username for the WordPress database
- `MYSQL_PASSWORD` — Password for the WordPress database

### Ports (optional)

By default, port **8000** is used for WordPress and **3306** for MySQL. If you prefer different ports, you can change them in your `.env` file.

## Run

After completing the steps above, you can start the containers:

```bash
docker compose up -d
```

Then visit [http://localhost:8000](http://localhost:8000)

## Contributing

Would you like to contribute to the development of this project? Then read the prepared [contribution guidelines](CONTRIBUTING.md) and go ahead!

Thank you for being involved! :heart_eyes:

## License

MIT License

Copyright (c) 2021-2025 Klaas Schoute

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
[maintenance-shield]: https://img.shields.io/maintenance/yes/2025.svg
[contributors-shield]: https://img.shields.io/github/contributors/klaasnicolaas/wordpress-docker.svg
[contributors-url]: https://github.com/klaasnicolaas/wordpress-docker/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/wordpress-docker.svg
[forks-url]: https://github.com/klaasnicolaas/wordpress-docker/network/members
[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/wordpress-docker.svg
[stars-url]: https://github.com/klaasnicolaas/wordpress-docker/stargazers
[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/wordpress-docker.svg
[issues-url]: https://github.com/klaasnicolaas/wordpress-docker/issues
[license-shield]: https://img.shields.io/github/license/klaasnicolaas/wordpress-docker.svg
[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/wordpress-docker.svg
[commits]: https://github.com/klaasnicolaas/wordpress-docker/commits/master
[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/wordpress-docker.svg