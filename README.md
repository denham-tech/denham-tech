# Denham Tech

Data pipeline engineering and headless extraction systems for e-commerce catalogs.

Specialized in deterministic schema validation, scheduled snapshot ingestion, relational delta computing, and event-driven alerting feeds for retail storefronts.

---

### Core Repositories & Modules

| Repository | Focus | Tech Stack |
| :--- | :--- | :--- |
| **[catalog-validation-sentinel](https://github.com/denham-tech/catalog-validation-sentinel)** | CLI data quality validator enforcing schema conformity, duplicate variant detection, and hygiene scoring. | Python, Pandas, Pytest |
| **[ecommerce-delta-engine](https://github.com/denham-tech/ecommerce-delta-engine)** | Relational snapshot diffing engine isolating SKU additions, delistings, price adjustments, and stockouts. | Python, Pandas, SQLite |
| **[automated-data-engine](https://github.com/denham-tech/automated-data-engine)** | Headless catalog scraper extracting paginated storefront inventories into structured relational feeds. | Python, Requests/HTTP, SQLite |
| **[ecom-telemetry-alerts](https://github.com/denham-tech/ecom-telemetry-alerts)** | Webhook routing module pushing catalog change payloads and error telemetry to operational channels. | Python, Webhooks/JSON |

---

### Architecture Standards
- **Relational Integrity:** Schema assertions prior to warehouse ingestion.
- **Deterministic Diffing:** Primary-key-based outer merges for catalog state tracking.
- **Configurable CLI & Logging:** Standard library logging, parameterized execution, and discrete test suites.
