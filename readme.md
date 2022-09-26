# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

- Create a .env file in the root of this project and pass in this values
```sh
POSTGRES_USER=myuser
POSTGRES_PASSWORD=mypassword
```
I used the default postgres user, and its password as it's setup on my pgAdmin

- run `docker-compose up` to build and run all containers
- Go to `http://localhost:3000/api/ping`. If you get a Pending Migrations error, sinply click run migration button available on the error page.
- If all is well, you should get something similar to this

```json
{"msg":"Pong! Seems like Everythink is working, great job!"}
```
