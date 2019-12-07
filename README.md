# Full-stack Python and Vue.js application

## Description

This project was generated using a [Cookiecutter](https://cookiecutter.readthedocs.io/en/latest/) template at [br3ndonland/full-stack-fastapi-postgresql](https://github.com/br3ndonland/full-stack-fastapi-postgresql) with:

```bash
cookiecutter https://github.com/br3ndonland/full-stack-fastapi-postgresql
```

See the template [repo](https://github.com/br3ndonland/full-stack-fastapi-postgresql) and [wiki](https://github.com/br3ndonland/full-stack-fastapi-postgresql/wiki) for more details on how to use the project.

See [CONTRIBUTING.md](./.github/CONTRIBUTING.md) for development methods and instructions for contributing to the project.

## Stack

### Back-end

- [FastAPI](fastapi.tiangolo.com/) is used as the back-end Python framework.
- PostgreSQL is used as the database.
- The application runs in several Docker containers using [Docker Compose](https://docs.docker.com/compose/), [Docker Stacks](https://docs.docker.com/compose/bundles/), and [Docker Swarm](https://dockerswarm.rocks/).
- Asynchronous background jobs can be run with [Celery](https://pypi.org/project/celery/) and [RabbitMQ](https://www.rabbitmq.com/).

### Front-end

- [Vue CLI](https://cli.vuejs.org/) 4 provides the base front-end application.
- [Vuetify](https://vuetifyjs.com/en/) provides a material design user interface component framework.
- The Vue.js components are built with [TypeScript](https://www.typescriptlang.org/).

## Quickstart

### Back-end requirements

- Docker
- Docker Compose

### Back-end instructions

Start the stack with Docker Compose:

```bash
docker-compose up -d
```

Now you can open your browser and interact with these URLs:

- Front-end, built with Docker, with routes handled based on the path: http://localhost
- Back-end, JSON based web API based on OpenAPI: http://localhost/api/
- Automatic interactive documentation with Swagger UI (from the OpenAPI backend): http://localhost/docs
- Alternative automatic documentation with ReDoc (from the OpenAPI backend): http://localhost/redoc
- PGAdmin, PostgreSQL web administration: http://localhost:5050
- Flower, administration of Celery tasks: http://localhost:5555
- Traefik UI, to see how the routes are being handled by the proxy: http://localhost:8090

### Front-end requirements

- Node.js (with `npm`)

### Front-end instructions

Enter the `frontend` directory, install the NPM packages and start the live server using the `npm` scripts:

```bash
cd frontend
npm install
npm run serve
```

Then open your browser at http://localhost:8080.
