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
* `respect`: Validates an OpenAPI implementation against the Arazzo description files located in the `arazzo` directory. This command assumes the API service is running on port `4010`, the same port used by the mock server.

Arazzo
------

The [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html) allows you to describe API workflows in both a human-readable and machine-readable format. This enhances API specifications by providing a narrative that improves the developer experience for those consuming the API.

As of this writing, the current version of the specification is **`1.0.1`**. You can find an Arazzo description in the `arazzo` directory, created to learn how the specification works in practice.

Arazzo is a promising young project. While it currently lacks some features found in tools like [Hurl](https://github.com/Orange-OpenSource/hurl) or [httpyac](https://github.com/anweber/httpyac), we'll continue to monitor its development as we continue to develop contract tests using other tool(s).

Documentation
-------------

Currently, the documentation is being built using [Redoc](https://github.com/Redocly/redoc). However, the following are alternative tools we could potentially use:

* [Zudoku](https://github.com/zuplo/zudoku)
* [xyd](https://github.com/livesession/xyd)
* [Scalar](https://github.com/scalar/scalar)
* [Stoplight Elements](https://github.com/stoplightio/elements)
* [Swagger UI](https://github.com/swagger-api/swagger-ui)
