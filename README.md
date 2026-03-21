# Deno (deno)
Deno is a modern JavaScript and TypeScript runtime built on V8 that emphasizes security, simplicity, and developer productivity. It provides a comprehensive developer platform including the Deno Deploy serverless edge network, a built-in key-value store, and a standard library of audited modules, all designed to run TypeScript natively without additional tooling.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - JavaScript, TypeScript, Runtime, Serverless, Edge, Deployment

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-03-21

## APIs

### Deno Runtime API
The Deno Runtime API is the built-in namespace of globals and modules available to all programs running on the Deno JavaScript and TypeScript runtime. It provides access to filesystem operations, networking, process management, cryptography, subprocesses, permissions, and environment variables via the Deno.* namespace. The runtime natively supports TypeScript without additional tooling and implements Web Platform APIs such as fetch, WebSocket, URL, and Web Crypto. Deno 2 introduced Node.js and npm compatibility, enabling use of the broader JavaScript ecosystem alongside the native Deno APIs.

**Human URL:** [https://docs.deno.com/api/deno/](https://docs.deno.com/api/deno/)


#### Tags:

 - JavaScript, TypeScript, Runtime, WebAssembly

#### Properties

- [Documentation](https://docs.deno.com/api/deno/)
- [JSONSchema](json-schema/deno-deployment-schema.json)

### Deno KV API
Deno KV is a key-value database built directly into the Deno runtime and available as a globally distributed store on Deno Deploy. It is accessed via the Deno.Kv namespace and supports get, set, delete, list, and atomic transaction operations. Keys are ordered tuples that support hierarchical data modeling, and values can be any structured-serializable JavaScript value including the special Deno.KvU64 type for 64-bit unsigned integers. When running locally, KV persists data using SQLite; on Deno Deploy, data is replicated across regions and accessible via a KV Connect URL in the format https://api.deno.com/databases/{database-id}/connect.

**Human URL:** [https://docs.deno.com/deploy/kv/](https://docs.deno.com/deploy/kv/)


#### Tags:

 - Key-Value, Database, Storage, Edge

#### Properties

- [Documentation](https://docs.deno.com/deploy/kv/)
- [Documentation](https://docs.deno.com/api/deno/~/Deno.Kv)
- [JSONSchema](json-schema/deno-kv-database-schema.json)

### Deno Deploy REST API
The Deno Deploy REST API provides programmatic access to manage projects and deployments on the Deno Deploy serverless edge platform. It exposes endpoints for creating and managing organizations, projects, deployments, domains, and KV databases, as well as retrieving analytics and usage metrics. The API base URL is https://api.deno.com/v1 and uses HTTP Bearer token authentication. An OpenAPI specification is published and can be used with OpenAPI-compatible tooling. This API covers the same operations available through the Deno Deploy dashboard.

**Human URL:** [https://docs.deno.com/deploy/api/rest/](https://docs.deno.com/deploy/api/rest/)


#### Tags:

 - Deployment, Serverless, Edge, Management

#### Properties

- [Documentation](https://docs.deno.com/deploy/api/rest/)
- [Documentation](https://apidocs.deno.com/)
- [OpenAPI](openapi/deno-deploy-rest-api-openapi.yml)

### Deno Deploy API v2
The Deno Deploy API v2 is the current generation REST API for managing applications, revisions, layers, and configuration on the Deno Deploy serverless edge platform. It replaces the v1 API (sunsetting July 20, 2026) with a revised resource model: Apps replace Projects, Revisions replace Deployments, and Layers provide reusable shared configuration across many apps. The v2 API introduces cursor-based pagination, streaming build progress via Server-Sent Events, and support for framework presets including Next.js, Astro, and Fresh.

**Human URL:** [https://api.deno.com/v2/docs](https://api.deno.com/v2/docs)


#### Tags:

 - Deployment, Serverless, Edge, Management

#### Properties

- [Documentation](https://api.deno.com/v2/docs)
- [OpenAPI](openapi/deno-deploy-v2-api-openapi.yml)

### Deno Subhosting API
The Deno Subhosting API enables platforms and SaaS products to run untrusted, user-submitted JavaScript and TypeScript code securely on Deno Deploy infrastructure. It shares the same base URL (https://api.deno.com/v1) and Bearer token authentication as the Deploy REST API but is scoped to subhosting use cases such as provisioning isolated projects per tenant, creating deployments, and managing custom domains and KV databases on behalf of end users. A JavaScript client library is available via the denoland/subhosting-js package, and a Python client is published on PyPI. Common use cases include cloud IDEs, no-code platforms, and multi-tenant application hosting.

**Human URL:** [https://docs.deno.com/subhosting/api/](https://docs.deno.com/subhosting/api/)


#### Tags:

 - Subhosting, Serverless, Multi-Tenant, Deployment

#### Properties

- [Documentation](https://docs.deno.com/subhosting/api/)
- [Documentation](https://docs.deno.com/subhosting/manual/)
- [OpenAPI](openapi/deno-subhosting-api-openapi.yml)

### Deno Standard Library
The Deno Standard Library is a collection of audited TypeScript modules maintained by the Deno core team and published on JSR under the @std scope. It provides common utilities including HTTP server helpers, path manipulation, assertions, CSV and JSON parsing, hashing, encoding, streams, date formatting, and more. All modules are guaranteed to work with the current stable Deno release and do not rely on third-party dependencies. Unlike Node.js built-ins, the standard library modules are imported by URL or JSR specifier, enabling version pinning and explicit dependency management.

**Human URL:** [https://docs.deno.com/runtime/fundamentals/standard_library/](https://docs.deno.com/runtime/fundamentals/standard_library/)


#### Tags:

 - Standard Library, Utilities, TypeScript, Modules

#### Properties

- [Documentation](https://docs.deno.com/runtime/fundamentals/standard_library/)
- [Documentation](https://jsr.io/@std)

## Common Properties

- [Website](https://deno.com)
- [Portal](https://dash.deno.com)
- [Documentation](https://docs.deno.com)
- [Blog](https://deno.com/blog)
- [Login](https://dash.deno.com/signin)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
