---
title: django-template
date: 2021-04-12T08:09:14+0000
draft: false
---
<p align="center">
<a href="https://dscvit.com">
	<img src="https://user-images.githubusercontent.com/30529572/92081025-fabe6f00-edb1-11ea-9169-4a8a61a5dd45.png" alt="DSC VIT"/>
</a>
	<h2 align="center"> django-template </h2>
	<h4 align="center"> An opinionated template for quickly getting started with Django <h4>
</p>

---
[![Join Us](https://img.shields.io/badge/Join%20Us-Developer%20Student%20Clubs-red)](https://dsc.community.dev/vellore-institute-of-technology/)
[![Discord Chat](https://img.shields.io/discord/760928671698649098.svg)](https://discord.com/invite/cWyEXgV)


## Features
- [x] Everything Django offers OOTB
- [x] CORS support  
- [x] Autogenerated OpenAPI and ReDoc API documentation
- [x] Production deployment using docker-compose
- [x] SSL using Nginx and LetsEncrypt

<br>


## Instructions to run

### Pre-requisites:
-  [Python 3.7 and above](https://www.python.org/downloads/)
-  [Poetry](https://python-poetry.org/)
-  [Docker](https://docs.docker.com/engine/install/)
-  [docker-compose](https://docs.docker.com/compose/install/)
	
### Installing dependencies
```bash
poetry shell # sets up and activates a venv
poetry install # installs missing dependencies from the lockfile
```

### Run migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### Start the server

In debug
```bash
python manage.py runserver
```

In production
```bash
docker-compose up -d --build
```

## More info
This template comes with an already existing model. Feel free to modify or remove it.

API docs can be found at:
- http://localhost:8000/docs (OpenAPI 3)
- http://localhost:8000/redoc (ReDoc)

## Contributors

<table>
<tr align="center">


<td>

Amogh Lele

<p align="center">
<img src = "https://avatars3.githubusercontent.com/u/31761843" width="150" height="150" alt="Amogh Lele">
</p>
<p align="center">
<a href = "https://github.com/atechnohazard"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36" alt="GitHub"/></a>
<a href = "https://www.linkedin.com/in/amogh-lele-830131a4/">
<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36" alt="LinkedIn"/>
</a>
</p>
</td>

  </table>

<p align="center">
	Made with :heart: by <a href="https://dscvit.com">DSC VIT</a>
</p>