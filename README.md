<div align="center">

<img src="./.github/assets/logo.svg" alt="awesome logo: a lens scans an index of packages and settles on the one that fits" width="140" height="140">

<h1>Awesome tada5hi</h1>

**Libraries, frameworks and tools built and maintained by [tada5hi](https://github.com/tada5hi).**

Before writing a utility from scratch, check here: there might already be a package for it.<br>
Includes the [authup](https://github.com/authup) and [routup](https://github.com/routup) ecosystems.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[Contents](#contents) · [Agent Skills](#agent-skills) · [Also Maintaining](#also-maintaining) · [License](#license)

</div>

---

<!-- package-list
Read by the query-package-list and refresh-package-list skills (https://github.com/tada5hi/skills).
Entry format, one line per repository, keep it strict:
- [name](https://github.com/owner/repo) `npm: pkg-a, pkg-b` – Short description ending with a period.
Install markers: npm, pypi, action, plugin. Monorepos list the packages a consumer installs, not every internal one.

owners: tada5hi, authup, routup
exclude:
- tada5hi/typescript-swagger: superseded by tada5hi/trapi
- tada5hi/docker-scan: superseded by tada5hi/docken
- tada5hi/monorepo-publish-action: superseded by tada5hi/monoship
- tada5hi/tada5hi: profile README
- tada5hi/typeorm-extension-test-esm: test fixture
- authup/documentation: docs site
- authup/helm: deployment
- authup/vue2: legacy backport
- routup/templates: starter templates
- tada5hi/awesome: this list
- @authup/*-console: console app bundles
- @authup/*-kit: internal toolkits, pulled in by the listed packages
- @authup/*-theme: pulled in by @authup/client-web-kit
- @authup/server-config: internal
- @authup/errors: internal
- @authup/kit: internal
- @authup/i18n: internal
- @authup/specs: internal
- @authup/server-adapter-socket-io: listed under authup/adapters
- @trapi/core: internal
- @vuecs/*: listed packages cover the entry points; components install on demand
- @tada5hi/eslint-config-*: replaced by @tada5hi/eslint-config
-->

## Contents

- [Databases & ORM](#databases--orm)
- [REST APIs & HTTP](#rest-apis--http)
- [Routing](#routing)
- [Authentication & Authorization](#authentication--authorization)
- [Validation & Errors](#validation--errors)
- [Objects & Data](#objects--data)
- [Application Structure & Messaging](#application-structure--messaging)
- [Configuration, Environment & Files](#configuration-environment--files)
- [Internationalization](#internationalization)
- [Frontend](#frontend)
- [Desktop](#desktop)
- [Text & Content](#text--content)
- [Docker, Helm & Releases](#docker-helm--releases)
- [Developer Tooling](#developer-tooling)
- [Agent Skills](#agent-skills)
- [Also Maintaining](#also-maintaining)

## Databases & ORM

- [typeorm-extension](https://github.com/tada5hi/typeorm-extension) `npm: typeorm-extension` – Create and drop databases, seed data sets and apply URL query parameters to TypeORM queries.
- [redis-extension](https://github.com/tada5hi/redis-extension) `npm: redis-extension` – Manage singleton Redis client and cluster instances, cache entities and track entity identifiers in groups.

## REST APIs & HTTP

- [rapiq](https://github.com/tada5hi/rapiq) `npm: @rapiq/core, @rapiq/codec-url, @rapiq/parser-simple, @rapiq/parser-expression, @rapiq/parser-mongo, @rapiq/adapter-typeorm, @rapiq/adapter-sql, @rapiq/adapter-drizzle, @rapiq/adapter-prisma, @rapiq/adapter-memory` – Typed REST queries (fields, filters, relations, pagination, sort) end-to-end: builders, parsers, URL codec and SQL, TypeORM, Drizzle, Prisma and in-memory adapters.
- [hapic](https://github.com/tada5hi/hapic) `npm: hapic, @hapic/oauth2, @hapic/vault, @hapic/harbor, @hapic/loki, @hapic/victorialogs` – Tiny fetch-based HTTP client with ready-made clients for OAuth2, Vault, Harbor, Loki and VictoriaLogs.
- [trapi](https://github.com/tada5hi/trapi) `npm: @trapi/cli, @trapi/metadata, @trapi/swagger, @trapi/preset-decorators-express, @trapi/preset-typescript-rest` – Generate REST API metadata and OpenAPI/Swagger documents from TypeScript decorators.

## Routing

- [routup](https://github.com/routup/routup) `npm: routup` – Fast, lightweight, runtime-agnostic and asynchronous routing framework.
- [routup plugins](https://github.com/routup/plugins) `npm: @routup/basic, @routup/body, @routup/cookie, @routup/query, @routup/cors, @routup/assets, @routup/decorators, @routup/i18n, @routup/logger, @routup/prometheus, @routup/rate-limit, @routup/rate-limit-redis, @routup/swagger-ui` – Body, cookie and query parsing, CORS, static assets, decorators, i18n, request logging, Prometheus metrics, rate limiting and Swagger UI for routup.

## Authentication & Authorization

- [authup](https://github.com/authup/authup) `npm: authup, create-authup, @authup/server-core, @authup/access, @authup/core-kit, @authup/core-http-kit, @authup/client-web-kit, @authup/client-web-nuxt, @authup/server-adapter-node, @authup/server-adapter-web` – Self-hosted IAM: OAuth2 and OpenID Connect provider with realms, RBAC and ABAC policies, MFA, admin and account consoles.
- [authup adapters](https://github.com/authup/adapters) `npm: @authup/server-adapter-http, @authup/server-adapter-socket-io, @authup/server-adapter-kit` – HTTP and Socket.IO adapters to protect services with authup.
- [authup python-sdk](https://github.com/authup/python-sdk) `pypi: authup` – Python plugins for authup: FastAPI, Flask, httpx and requests integrations.

## Validation & Errors

- [validup](https://github.com/tada5hi/validup) `npm: validup, @validup/zod, @validup/standard-schema, @validup/validator-js, @validup/vue` – Compose validators and nested containers onto object paths, with Zod, Standard Schema, validator.js and Vue 3 integrations.
- [ebec](https://github.com/tada5hi/ebec) `npm: @ebec/core, @ebec/http` – Extensible, type-safe error classes with code derivation, message interpolation, grouping, JSON serialization and 43 ready-made HTTP errors.
- [blemish](https://github.com/tada5hi/blemish) `npm: blemish` – Dependency-free issue tree model: nested item/group issues with absolute paths, shared across validation libraries.

## Objects & Data

- [smob](https://github.com/tada5hi/smob) `npm: smob` – Zero-dependency, safe deep merge of objects and arrays with customizable behavior.
- [pathtrace](https://github.com/tada5hi/pathtrace) `npm: pathtrace` – Get, set and check values at any path in nested objects and arrays.
- [dycraft](https://github.com/tada5hi/dycraft) `npm: dycraft` – Shape objects dynamically with default values and getters.
- [continu](https://github.com/tada5hi/continu) `npm: continu` – Zero-dependency key-value container with defaults, transformers and validators for nested options.
- [twinop](https://github.com/tada5hi/twinop) `npm: twinop` – Derive parallel sync and async APIs from one shared generator body.

## Application Structure & Messaging

- [eldin](https://github.com/tada5hi/eldin) `npm: eldin` – Lightweight, type-safe dependency injection container with scoped lifetimes and hierarchical containers.
- [orkos](https://github.com/tada5hi/orkos) `npm: orkos` – Modular application orchestrator with dependency-ordered startup and shutdown.
- [singa](https://github.com/tada5hi/singa) `npm: singa` – Tiny library to create and manage singleton instances.
- [hubwire](https://github.com/tada5hi/hubwire) `npm: hubwire, @hubwire/amqp, @hubwire/test` – Components with a start/stop/status lifecycle, command handlers, scheduled jobs and a message bus routing commands between them.
- [amqp-extension](https://github.com/tada5hi/amqp-extension) `npm: amqp-extension` – Publish and consume RabbitMQ messages without amqplib boilerplate: reconnects, exchange and queue setup, payload encoding.

## Configuration, Environment & Files

- [confinity](https://github.com/tada5hi/confinity) `npm: confinity` – Load and merge configuration across a multi-package application from .conf, JSON, YAML and TS/JS files.
- [envix](https://github.com/tada5hi/envix) `npm: envix` – Read, transform and require environment variables across Node.js, Deno, Bun and the browser.
- [locter](https://github.com/tada5hi/locter) `npm: locter` – Locate files with glob patterns and read or write them by format (JSON, YAML, conf, text, TS/JS modules).

## Internationalization

- [ilingo](https://github.com/tada5hi/ilingo) `npm: ilingo, @ilingo/fs, @ilingo/vue, @ilingo/validup, @ilingo/validup-vue, @ilingo/vuelidate` – Lightweight, framework-agnostic translation library with file-system store, Vue 3, validup and Vuelidate integrations.

## Frontend

- [vuecs](https://github.com/tada5hi/vuecs) `npm: @vuecs/core, @vuecs/design, @vuecs/theme-tailwind, @vuecs/theme-bootstrap, @vuecs/theme-bulma, @vuecs/nuxt, @vuecs/forms, @vuecs/table, @vuecs/list, @vuecs/overlays, @vuecs/navigation, @vuecs/pagination, @vuecs/tree` – Vue 3 theming framework: themeable components, design tokens, dark mode and runtime palettes with Tailwind, Bootstrap and Bulma themes.
- [browser-storage-adapter](https://github.com/tada5hi/browser-storage-adapter) `npm: browser-storage-adapter` – Save key-value pairs to one or many browser stores at once (localStorage, sessionStorage, cookies).

## Desktop

- [vitron](https://github.com/tada5hi/vitron) `npm: vitron` – Build Windows, Linux and macOS desktop apps from modern web projects with Vite and Electron.

## Text & Content

- [bulletin-board-code](https://github.com/tada5hi/bulletin-board-code) `npm: bulletin-board-code` – Convert BBCode to HTML and back.
- [mime-explorer](https://github.com/tada5hi/mime-explorer) `npm: mime-explorer` – Look up MIME types by path or extension, with meta information and standard extensions per type.

## Docker, Helm & Releases

- [docken](https://github.com/tada5hi/docken) `npm: docken` – Utilities on top of dockerode, including scanning organized Dockerfiles on the file system.
- [craneship](https://github.com/tada5hi/craneship) `npm: craneship` – Build, tag and push Docker images with tags derived from the git ref, as GitHub Action, CLI and library.
- [hevi](https://github.com/tada5hi/hevi) `npm: hevi` – Version and release Helm charts: bump versions across file:// dependencies, push to OCI registries and GitHub Pages.
- [hevi-action](https://github.com/tada5hi/hevi-action) `action: tada5hi/hevi-action` – GitHub Action to run hevi.
- [monoship](https://github.com/tada5hi/monoship) `npm: monoship` – Publish only the npm workspace packages the registry is missing, resolving workspace: dependencies and supporting OIDC trusted publishing.

## Developer Tooling

- [javascript](https://github.com/tada5hi/javascript) `npm: @tada5hi/eslint-config, @tada5hi/prettier-config, @tada5hi/commitlint-config, @tada5hi/tsconfig, @tada5hi/semantic-release` – Shared ESLint (TypeScript and Vue), Prettier, commitlint, tsconfig and semantic-release configurations.

## Agent Skills

- [skills](https://github.com/tada5hi/skills) `plugin: tada5hi/skills` – Curated agent skills for Claude Code and other agents: agent docs, READMEs, release notes, PR review triage, type audits and more.

## Also Maintaining

- [rollup/plugins](https://github.com/rollup/plugins) `npm: @rollup/plugin-*` – The official Rollup plugins.
- [eslint-config-rollup](https://github.com/rollup/eslint-config-rollup) `npm: eslint-config-rollup` – Shareable ESLint configuration for Rollup projects.

## License

[CC0 1.0](LICENSE): to the extent possible under law, tada5hi has waived all copyright and related rights to this list.
