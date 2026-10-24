<p align="center"><a href="https://kinetis.dev" target="_blank"><img src="logo.svg" alt="Kinetis" width="320"></a></p>

## About Kinetis

Kinetis is a PHP framework for API-first applications, built for persistent workers and non-blocking I/O. A slow database query or a flaky third-party API suspends a Fiber, not the whole worker, so one slow request never holds up the requests behind it. Everything you need to build an API comes in the box:

- [Attribute-based routing and validation](https://kinetis.dev/docs/routing-validation.html), with typed request DTOs. A malformed request gets a 422 before your controller runs.
- [OpenAPI 3.1 and Swagger UI](https://kinetis.dev/docs/routing-validation.html#openapi-documentation), generated from your route attributes.
- [Fiber-based concurrency](https://kinetis.dev/docs/concurrency.html) over the Revolt event loop, with non-blocking MySQL, Postgres and Redis drivers.
- A [two-tier dependency injection container](https://kinetis.dev/docs/container.html) that enforces request-scope isolation.
- A [native Model Context Protocol server](https://kinetis.dev/docs/mcp.html), so AI agents can call your application's tools and resources.
- [Authentication](https://kinetis.dev/docs/auth.html) with bearer tokens or [JWT](https://kinetis.dev/docs/auth-jwt.html), plus [authorization](https://kinetis.dev/docs/authorization.html) and [sessions with CSRF protection](https://kinetis.dev/docs/session.html).
- A [data mapper ORM](https://kinetis.dev/docs/orm.html), a [query builder](https://kinetis.dev/docs/query-builder.html) and [migrations](https://kinetis.dev/docs/migrations.html).
- [Background jobs](https://kinetis.dev/docs/queue.html) on Redis, SQL, Amazon SQS or RabbitMQ.
- [File storage](https://kinetis.dev/docs/storage.html), [mail](https://kinetis.dev/docs/mailer.html), [search](https://kinetis.dev/docs/search-engines.html), [real-time broadcasting](https://kinetis.dev/docs/broadcasting.html) and [OpenTelemetry tracing](https://kinetis.dev/docs/telemetry.html).

The same application code runs unchanged on [FrankenPHP, RoadRunner, PHP-FPM or AWS Lambda](https://kinetis.dev/docs/runtime-adapters.html). Start simple, and move to a persistent worker when you need one.

## Learning Kinetis

The [documentation](https://kinetis.dev/docs/) covers every package in one place. The [tutorial](https://kinetis.dev/docs/tutorial.html) gets a route running in minutes, then walks you through a real application with a database, a queue, a scheduled command and live updates.

To start a project, use [`kinetis/skeleton`](https://github.com/kinetis-dev/skeleton), the smallest runnable Kinetis application. For a complete example, see [`kinetis/pingpong`](https://github.com/kinetis-dev/pingpong). It covers MySQL, queues, events, cron, an MCP tool and live WebSocket updates.

Want to compare performance? The [benchmarks](https://kinetis.dev/docs/benchmarks.html) are an auditable, cross-framework suite, and their methodology is published alongside the results.

## Contributing

Kinetis is developed in the [kinetis-dev/kinetis](https://github.com/kinetis-dev/kinetis) monorepo. Each package is split out from there into its own repository. Please see the [contribution guide](https://kinetis.dev/docs/appendix-contributing.html) and the [security policy](https://github.com/kinetis-dev/kinetis/blob/main/SECURITY.md).

Kinetis is open-source software licensed under the [MIT license](https://github.com/kinetis-dev/kinetis/blob/main/LICENSE).
