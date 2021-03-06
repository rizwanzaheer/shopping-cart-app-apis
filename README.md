## Quick Start

Install the dependencies:

```bash
yarn install
```

Set the environment variables:

```bash
cp .env.example .env

# open .env and modify the environment variables (if needed)
```


## Commands

Running locally:

```bash
yarn dev
```

Running in production:

```bash
yarn start
```

Linting:

```bash
# run ESLint
yarn lint

# fix ESLint errors
yarn lint:fix

# run prettier
yarn prettier

# fix prettier errors
yarn prettier:fix
```

## Environment Variables

The environment variables can be found and modified in the `.env` file. They come with these default values:

```bash

# Port number
PORT=3000

# URL of the Mongo DB
MONGODB_URL=mongodb://127.0.0.1:27017/exampleDataBase

# BaseURL of domain
BASE_URL=localhost


```

## Project Structure

```
src\
 |--config\         # Environment variables and configuration related things
 |--controllers\    # Route controllers (controller layer)
 |--docs\           # Swagger files
 |--middlewares\    # Custom express middlewares
 |--models\         # Mongoose models (data layer)
 |--routes\         # Routes
 |--services\       # Business logic (service layer)
 |--utils\          # Utility classes and functions
 |--db\             # Test dump db files
 |--postman\        # Postman file all APIs with test data
 |--validations\    # Request data validation schemas
 |--app.js          # Express app
 |--index.js        # App entry point
```

## API Documentation

To view the list of available APIs and their specifications, run the server and go to `http://localhost:3000/api/v1/docs` in your browser. This documentation page is automatically generated using the [swagger](https://swagger.io/) definitions written as comments in the route files.

