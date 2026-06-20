# Memgraph (memgraph)

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
