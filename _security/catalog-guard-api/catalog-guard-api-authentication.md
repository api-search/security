---
api_key_in: []
api_specs:
- filename: catalog-guard-api-catalog-api-openapi.yml
  format: yaml
  label: Catalog Guard API Catalog API
  slug: catalog-guard-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catalog-guard-api/refs/heads/main/openapi/catalog-guard-api-catalog-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Catalog Guard Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Catalog Guard API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Catalog Guard API
provider_slug: catalog-guard-api
scheme_count: 0
schemes: []
slug: catalog-guard-api-authentication
source_filename: catalog-guard-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: >-\n  https://catalogguard.noahcortezj-c.workers.dev/api/v1/catalog/docs,\n  https://catalogguard.noahcortezj-c.workers.dev/openapi.json,\n  https://catalogguard.noahcortezj-c.workers.dev/privacy\ndocs: https://catalogguard.noahcortezj-c.workers.dev/api/v1/catalog/docs\nsummary:\n  model: none\n  types: []\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\ndetail: >-\n  This API is deliberately and explicitly unauthenticated. The OpenAPI 3.1.0 document declares\n  no components.securitySchemes and neither operation carries a security requirement; a POST\n  with no credential of any kind returns 200. This was verified live, not assumed from an\n  empty spec.\n\n  The absence is a stated product position rather than an oversight. The docs endpoint ends\n  with the line \"No uploads, credentials, payment data, storage, store connection, or import.\"\n  Every successful response repeats it as machine-readable `disclosures`\n \
  \ (noCredentialsOrPaymentData, noStoreConnectionOrImport). The privacy page states the free\n  preflight processes CSV text in the browser and that Catalog Guard does not ask for store\n  credentials or retain CSV contents.\naccess_control:\n  mechanism: input bounds and best-effort rate limiting, not identity\n  detail: >-\n    With no identity layer, abuse control is entirely bound-based: 250 rows or 98304 CSV\n    characters per request, a 131072-byte body ceiling, strict content-type enforcement, and a\n    best-effort 20 requests/minute per Cloudflare isolate returning 429. There is no per-caller\n    quota, no attribution, and no way to revoke a specific consumer.\nagent_guidance: >-\n  An agent needs no credential setup, no key rotation and no consent flow to call this API.\n  The corresponding caveat is that there is no tenancy: nothing the API returns is scoped to a\n  caller, and nothing sent to it can be retrieved later.\nsignup_required: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalog-guard-api/refs/heads/main/authentication/catalog-guard-api-authentication.yml
summary_line: 0 schemes
tags:
- ecommerce
- catalog-validation
- shopify
- data-quality
- csv-validation
- product-data-qa
- data-preflight
- data-validation
- retail
---
