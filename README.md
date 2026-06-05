# Deno (deno)

Deno is a modern JavaScript and TypeScript runtime built on V8 that emphasizes security, simplicity, and developer productivity. It provides a comprehensive developer platform including the Deno Deploy serverless edge network, a built-in key-value store, and a standard library of audited modules, all designed to run TypeScript natively without additional tooling.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Producer
- **Access:** 3rd-Party

## Tags

- Deployment
- Edge
- JavaScript
- Runtime
- Serverless
- TypeScript

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-05-19

## APIs

### Deno Runtime API

The Deno Runtime API is the built-in namespace of globals and modules available to all programs running on the Deno JavaScript and TypeScript runtime. It provides access to filesystem operations, networking, process management, cryptography, subprocesses, permissions, and environment variables via the Deno.* namespace. The runtime natively supports TypeScript without additional tooling and implements Web Platform APIs such as fetch, WebSocket, URL, and Web Crypto.

- **Human URL:** [https://docs.deno.com/api/deno/](https://docs.deno.com/api/deno/)
- **Base URL:** `https://api.example.com`

#### Tags

- JavaScript
- Runtime
- TypeScript
- WebAssembly

#### Properties

- [Documentation](https://docs.deno.com/api/deno/)
- [JSON Schema](json-schema/deno-deployment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/deno-deploy-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-deploy-v2-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-v2-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-subhosting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-subhosting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deno KV API

Deno KV is a key-value database built directly into the Deno runtime and available as a globally distributed store on Deno Deploy. It is accessed via the Deno.Kv namespace and supports get, set, delete, list, and atomic transaction operations. Keys are ordered tuples that support hierarchical data modeling, and values can be any structured-serializable JavaScript value including the special Deno.KvU64 type for 64-bit unsigned integers.

- **Human URL:** [https://docs.deno.com/deploy/kv/](https://docs.deno.com/deploy/kv/)
- **Base URL:** `https://api.deno.com`

#### Tags

- Database
- Edge
- Key-Value
- Storage

#### Properties

- [Documentation](https://docs.deno.com/deploy/kv/)
- [Documentation](https://docs.deno.com/api/deno/~/Deno.Kv)
- [JSON Schema](json-schema/deno-kv-database-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/deno-deploy-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-deploy-v2-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-v2-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-subhosting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-subhosting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deno Deploy REST API

The Deno Deploy REST API provides programmatic access to manage projects and deployments on the Deno Deploy serverless edge platform. It exposes endpoints for creating and managing organizations, projects, deployments, domains, and KV databases, as well as retrieving analytics and usage metrics. The API base URL is https://api.deno.com/v1 and uses HTTP Bearer token authentication. An OpenAPI specification is published and can be used with OpenAPI-compatible tooling.

- **Human URL:** [https://docs.deno.com/deploy/api/rest/](https://docs.deno.com/deploy/api/rest/)
- **Base URL:** `https://api.deno.com/v1`

#### Tags

- Deployment
- Edge
- Management
- Serverless

#### Properties

- [Documentation](https://docs.deno.com/deploy/api/rest/)
- [Documentation](https://apidocs.deno.com/)
- [OpenAPI](openapi/deno-deploy-rest-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deno-deploy-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deno Deploy API V2

The Deno Deploy API v2 is the current generation REST API for managing applications, revisions, layers, and configuration on the Deno Deploy serverless edge platform. It replaces the v1 API (sunsetting July 20, 2026) with a revised resource model: Apps replace Projects, Revisions replace Deployments, and Layers provide reusable shared configuration across many apps.

- **Human URL:** [https://api.deno.com/v2/docs](https://api.deno.com/v2/docs)
- **Base URL:** `https://api.deno.com/v2`

#### Tags

- Deployment
- Edge
- Management
- Serverless

#### Properties

- [Documentation](https://api.deno.com/v2/docs)
- [OpenAPI](openapi/deno-deploy-v2-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deno-deploy-v2-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-v2-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deno Subhosting API

The Deno Subhosting API enables platforms and SaaS products to run untrusted, user-submitted JavaScript and TypeScript code securely on Deno Deploy infrastructure. It shares the same base URL (https://api.deno.com/v1) and Bearer token authentication as the Deploy REST API but is scoped to subhosting use cases such as provisioning isolated projects per tenant, creating deployments, and managing custom domains and KV databases on behalf of end users.

- **Human URL:** [https://docs.deno.com/subhosting/api/](https://docs.deno.com/subhosting/api/)
- **Base URL:** `https://api.deno.com/v1`

#### Tags

- Deployment
- Multi-Tenant
- Serverless
- Subhosting

#### Properties

- [Documentation](https://docs.deno.com/subhosting/api/)
- [Documentation](https://docs.deno.com/subhosting/manual/)
- [OpenAPI](openapi/deno-subhosting-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/deno-subhosting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-subhosting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Deno Standard Library

The Deno Standard Library is a collection of audited TypeScript modules maintained by the Deno core team and published on JSR under the @std scope. It provides common utilities including HTTP server helpers, path manipulation, assertions, CSV and JSON parsing, hashing, encoding, streams, date formatting, and more. All modules are guaranteed to work with the current stable Deno release and do not rely on third-party dependencies.

- **Human URL:** [https://docs.deno.com/runtime/fundamentals/standard_library/](https://docs.deno.com/runtime/fundamentals/standard_library/)
- **Base URL:** `https://api.example.com`

#### Tags

- Modules
- Standard Library
- TypeScript
- Utilities

#### Properties

- [Documentation](https://docs.deno.com/runtime/fundamentals/standard_library/)
- [Documentation](https://jsr.io/@std)
- [Postman Collection](collections/deno-deploy-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-deploy-v2-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-deploy-v2-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/deno-subhosting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/deno-subhosting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/deno)
- [Website](https://deno.com)
- [Portal](https://dash.deno.com)
- [Documentation](https://docs.deno.com)
- [Blog](https://deno.com/blog)
- [GitHub Organization](https://github.com/denoland)
- [Login](https://dash.deno.com/signin)
- [JSON-LD](json-ld/deno-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/deno-deployment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/deno-kv-database-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Vocabulary](vocabulary/deno-vocabulary.yml)
- [Capabilities](capabilities/deno-capabilities.yml)
- [Rules](rules/deno-rules.yml)
- [Integrations](https://deno.com/integrations)
- [L L Ms Txt](https://docs.deno.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
