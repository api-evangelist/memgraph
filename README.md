# Memgraph (memgraph)

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

Memgraph is an open-source, high-performance in-memory graph database built in C++ for real-time graph analytics, GraphRAG, and agentic AI. Its primary interface is Cypher executed over the Bolt wire protocol (TCP port 7687) via standard graph drivers - it is not a REST API. Memgraph also ships MAGE graph algorithms, the GQLAlchemy Python OGM, the Memgraph Lab visual interface, a WebSocket log-monitoring channel, and an Enterprise Prometheus-style metrics HTTP endpoint.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/memgraph/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/memgraph/refs/heads/main/apis.yml)

## Tags

- Graph Database
- In-Memory
- Cypher
- Bolt
- Real-Time

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Memgraph Bolt/Cypher Query Interface

The primary programmatic interface to Memgraph. Clients send openCypher queries over the binary Bolt protocol on TCP port 7687 (bolt:// or bolt+s://) using official Neo4j-compatible drivers for Python, JavaScript, Java, Go, Rust, C#, and PHP. This is a stateful wire protocol, not a REST/HTTP API; there are no HTTP query endpoints.

- **Human URL:** [https://memgraph.com/docs/querying](https://memgraph.com/docs/querying)
- **Base URL:** `bolt://localhost:7687`

#### Tags

- Cypher
- Bolt
- Query
- Graph

#### Properties

- [Documentation](https://memgraph.com/docs/client-libraries)
- [API Reference](https://memgraph.com/docs/querying)
- [OpenAPI](openapi/memgraph-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [GitHub](https://github.com/memgraph/memgraph)
- [Postman Collection](collections/memgraph.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/memgraph.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Memgraph MAGE Algorithms

MAGE (Memgraph Advanced Graph Extensions) is an open-source library of graph algorithms and query modules - traditional, dynamic, and ML-driven - invoked as Cypher procedures (CALL ...) over the same Bolt interface. Not a standalone HTTP API.

- **Human URL:** [https://memgraph.com/docs/advanced-algorithms](https://memgraph.com/docs/advanced-algorithms)
- **Base URL:** `bolt://localhost:7687`

#### Tags

- MAGE
- Algorithms
- Query Modules

#### Properties

- [Documentation](https://memgraph.com/docs/advanced-algorithms)
- [API Reference](https://memgraph.com/docs/advanced-algorithms/available-algorithms)
- [GitHub](https://github.com/memgraph/mage)
- [Postman Collection](collections/memgraph.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/memgraph.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Memgraph Monitoring and Metrics

Two operational surfaces. A WebSocket log channel (ws:// or wss:// on default 0.0.0.0:7444) streams real-time log messages to connected clients. An Enterprise-only metrics HTTP endpoint (default 0.0.0.0:9091) exposes system, query, transaction, and memory metrics in OpenMetrics/Prometheus format via GET.

- **Human URL:** [https://memgraph.com/docs/database-management/monitoring](https://memgraph.com/docs/database-management/monitoring)
- **Base URL:** `http://localhost:9091`

#### Tags

- Monitoring
- Metrics
- Prometheus
- WebSocket

#### Properties

- [Documentation](https://memgraph.com/docs/database-management/monitoring)
- [API Reference](https://memgraph.com/docs/configuration/server-stats)
- [OpenAPI](openapi/memgraph-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [GitHub](https://github.com/memgraph/memgraph)
- [Postman Collection](collections/memgraph.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/memgraph.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Memgraph Lab

Memgraph Lab is a lightweight visual interface for writing Cypher queries, visualizing graph results, importing data, and inspecting query modules. The Lab application itself connects to Memgraph over the Bolt protocol on port 7687; it is a client UI, not a public REST API.

- **Human URL:** [https://memgraph.com/docs/data-visualization](https://memgraph.com/docs/data-visualization)
- **Base URL:** `bolt://localhost:7687`

#### Tags

- Lab
- Visualization
- UI

#### Properties

- [Documentation](https://memgraph.com/docs/data-visualization)
- [GitHub](https://github.com/memgraph/lab)
- [Postman Collection](collections/memgraph.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/memgraph.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/memgraph)
- [LinkedIn](https://www.linkedin.com/company/memgraph)
- [Website](https://memgraph.com)
- [Documentation](https://memgraph.com/docs)
- [Plans](plans/memgraph-plans-pricing.yml)
- [Rate Limits](rate-limits/memgraph-rate-limits.yml)
- [Fin Ops](finops/memgraph-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
