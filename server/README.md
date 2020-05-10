
## Installation

```bash
$ npm install
```

## Running the app (without docker)

### Migrations
Make sure you have a PostgreSQL server available and set the `DATABASE_URL` environment variable to point to that Postgres instance, like:

```bash
$ cd server/src/
# run migrations (using [knex-migrate](https://github.com/sheerun/knex-migrate))
$ export DATABASE_URL=postgres://admin:5UPP3rSecr3tPAssword@localhost:54320/knests && knex-migrate up
```

Also, there's an API endpoint that runs the migrations once the app is started:
`GET http://localhost:8000/system/migrate`

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Development workflow


## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- knests - [Tudor Constantin](https://programming.tudorconstantin.com)
- NestJS Website - [https://nestjs.com](https://nestjs.com/)
