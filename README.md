# Basic project with Flask , Connexion and OpenApi 3

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/6d2db9a0569640ca86718aa670d8bfa9)](https://www.codacy.com/manual/cblack34/python-flask-connexion-example-openapi3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cblack34/python-flask-connexion-example-openapi3&amp;utm_campaign=Badge_Grade)
[![Build Status](https://travis-ci.org/cblack34/python-flask-connexion-example-openapi3.svg?branch=master)](https://travis-ci.org/cblack34/python-flask-connexion-example-openapi3)

Basic Python project using Flask and Connexion by Zalando

```http
https://github.com/zalando/connexion
```

## Requirements

*  Docker Compose 1.21.2+
*  Python 3.6 +

## Run with Docker Compose

```bash
# building the container
sudo docker-compose build

# starting up a container
sudo docker-compose up
```

## Build the virtual environment

```bash
virtualenv -p /usr/bin/python3.6 venv
source venv/bin/activate
pip3 install -r requirements.txt
pip3 install -r test-requirements.txt
```

## Swagger definition

```http
http://localhost:8081/v1/swagger.json
```

## Health Check

```http
http://localhost:8081/v1/basic/ping
```

## Launch tests

```bash
source venv/bin/activate
tox
```
