DockerPage
====
[![Version](https://img.shields.io/badge/SSERAFIM-OK-gree)](https://github.com/Sota-Nakashima/SSERAFIM)
[![Version](https://img.shields.io/badge/AESPA-OK-gree)](https://github.com/Sota-Nakashima/AESPA)
[![CC0 License](http://img.shields.io/badge/license-CC0-blue.svg?style=flat)](https://github.com/Sota-Nakashima/Docker/blob/main/LICENCE)
#  Overview
DockerFile repository

## Usage
1. Select the appropriate branch and clone in your disk.
2. Go to directory and run docker-compose command.
   ```bash:usage1.sh
   cd ~/Docker
   ```
   ```bash:usage2.sh
   docker-compose up --no-start
   ```
   ```bash:usage3.sh
   docker run -it --rm {hoge} /bin/bash
   ```
* The download directory and work directory are bind-mounted. Here you can put the necessary files or save the results to your disk.

## Requirement
* [Docker](https://github.com/docker)
* [Docker Compose](https://github.com/docker/compose)
## Licence

[CC0](https://github.com/Sota-Nakashima/Docker/blob/main/LICENCE)

## Author

[Sota Nakashima](https://github.com/Sota-Nakashima)