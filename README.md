# Deno (deno)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
