RouteHub OpenAPI Description
============================

This repository provides the OpenAPI description (OAD) for the RouteHub REST API. The documentation, generated from the OAD, can be found [here](https://tandiljuan.github.io/routehub-openapi/).

RouteHub is a service designed to optimize delivery routes based on a given set of deliveries, drivers, vehicle fleet and dispatch locations.

The project uses [Semantic Versioning](https://semver.org) to define how version numbers are assigned and incremented.

Development Tools
-----------------

### Core Dependencies

To ensure optimal performance and functionality, the following Node.js and NPM versions are required:

- [Node.js](https://nodejs.org/en) >= 20.19
- [NPM](https://www.npmjs.com) >= 10

The previous Node.js version was obtained using the command `npx ls-engines --dev`.

### Application Dependencies

Install the application's dependencies using `npm`:

```bash
npm install
```

### NPM Scripts

Below is a list of npm scripts (aliases) for frequently used commands. As a quick reference, remember to prepend `npm run` when executing these scripts.

* `lint`: Analyzes the OpenAPI description to identify potential errors.
* `bundle-yaml`: Bundles all files belonging to the OpenAPI description into a single YAML file.
* `bundle-json`: Bundles all files belonging to the OpenAPI description into a single JSON file.
* `build-man`: Generates documentation from the OpenAPI description.
* `mock`: Run mock service from the OpenAPI description.

Documentation
-------------

Currently, the documentation is being built using [Redoc](https://github.com/Redocly/redoc). However, the following are alternative tools we could potentially use:

* [Zudoku](https://github.com/zuplo/zudoku)
* [xyd](https://github.com/livesession/xyd)
* [Scalar](https://github.com/scalar/scalar)
* [Stoplight Elements](https://github.com/stoplightio/elements)
* [Swagger UI](https://github.com/swagger-api/swagger-ui)
