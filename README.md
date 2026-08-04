# Cloudprinter (cloudprinter)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
