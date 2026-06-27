# Cloudprinter (cloudprinter)

Cloudprinter.com is a global print-on-demand and print-fulfillment API network connecting buyers to 170+ print partners worldwide. The CloudCore REST API lets developers fetch product catalogs, request real-time price and shipping quotes, submit and manage print orders, and receive production and shipment events via CloudSignal webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/apis.yml)

## Tags

- Print on Demand
- Print Fulfillment
- Printing
- Orders
- Logistics

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### Cloudprinter Orders API

Create, list, retrieve, cancel, and audit print orders. Orders carry items, addresses, shipping levels, options, and file references, and are submitted as JSON POST requests with the CloudCore apikey in the body.

- **Human URL:** [https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- **Base URL:** `https://api.cloudprinter.com/cloudcore/1.0`

#### Tags

- Orders
- Fulfillment
- Printing

#### Properties

- [Documentation](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- [API Reference](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- [OpenAPI](openapi/cloudprinter-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudprinter.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudprinter.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudprinter Products & Pricing API

List products enabled for the account and retrieve detailed product specifications, available options, and pricing via the products and products/info endpoints.

- **Human URL:** [https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- **Base URL:** `https://api.cloudprinter.com/cloudcore/1.0`

#### Tags

- Products
- Catalog
- Pricing

#### Properties

- [Documentation](https://docs.cloudprinter.com/client/how-to-check-prices)
- [API Reference](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- [OpenAPI](openapi/cloudprinter-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudprinter.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudprinter.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudprinter Quotes API

Request real-time quotes for a list of items returning product prices, shipping options, and shipping prices. Each quote carries a unique hash valid for 48 hours that can be referenced when placing an order.

- **Human URL:** [https://docs.cloudprinter.com/client/how-to-check-prices](https://docs.cloudprinter.com/client/how-to-check-prices)
- **Base URL:** `https://api.cloudprinter.com/cloudcore/1.0`

#### Tags

- Quotes
- Pricing
- Shipping

#### Properties

- [Documentation](https://docs.cloudprinter.com/client/how-to-check-prices)
- [API Reference](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- [OpenAPI](openapi/cloudprinter-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudprinter.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudprinter.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudprinter Signal Webhooks API

CloudSignal pushes item-based production and shipment events (order validated, item produced, item shipped with tracking, item error, item cancelled) as small JSON POSTs to a configured CloudCore API interface, retrying up to 100 attempts over 7 days until a 200/204 is returned.

- **Human URL:** [https://docs.cloudprinter.com/client/cloudsignal-webhooks](https://docs.cloudprinter.com/client/cloudsignal-webhooks)
- **Base URL:** `https://api.cloudprinter.com/cloudcore/1.0`

#### Tags

- Webhooks
- Signals
- Events

#### Properties

- [Documentation](https://docs.cloudprinter.com/client/cloudsignal-webhooks)
- [OpenAPI](openapi/cloudprinter-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudprinter.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudprinter.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudprinter Files API

Print-ready files (product, cover, book) are referenced on order items by type, URL, and MD5 checksum, and are returned with the same metadata on order info for download and verification by production.

- **Human URL:** [https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- **Base URL:** `https://api.cloudprinter.com/cloudcore/1.0`

#### Tags

- Files
- Print Files
- Assets

#### Properties

- [Documentation](https://docs.cloudprinter.com/client/cloudprinter-core-api-v1-0/)
- [OpenAPI](openapi/cloudprinter-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudprinter.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudprinter.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/cloudprintercom)
- [LinkedIn](https://www.linkedin.com/company/cloudprinter-com)
- [Website](https://www.cloudprinter.com)
- [Documentation](https://docs.cloudprinter.com)
- [Plans](plans/cloudprinter-plans-pricing.yml)
- [Rate Limits](rate-limits/cloudprinter-rate-limits.yml)
- [Fin Ops](finops/cloudprinter-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
