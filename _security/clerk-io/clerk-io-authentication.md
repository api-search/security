---
api_key_in:
- query
- body
api_specs:
- filename: clerk-io-accessories-api-openapi.yml
  format: yaml
  label: Clerk.io Accessories API
  slug: clerk-io-accessories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-accessories-api-openapi.yml
- filename: clerk-io-audiences-api-openapi.yml
  format: yaml
  label: Clerk.io Audiences API
  slug: clerk-io-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-audiences-api-openapi.yml
- filename: clerk-io-campaigns-api-openapi.yml
  format: yaml
  label: Clerk.io Campaigns API
  slug: clerk-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-campaigns-api-openapi.yml
- filename: clerk-io-catalog-api-openapi.yml
  format: yaml
  label: Clerk.io Catalog API
  slug: clerk-io-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-catalog-api-openapi.yml
- filename: clerk-io-logging-api-openapi.yml
  format: yaml
  label: Clerk.io Logging API
  slug: clerk-io-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-logging-api-openapi.yml
- filename: clerk-io-merchandising-api-openapi.yml
  format: yaml
  label: Clerk.io Merchandising API
  slug: clerk-io-merchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-merchandising-api-openapi.yml
- filename: clerk-io-parcels-api-openapi.yml
  format: yaml
  label: Clerk.io Parcels API
  slug: clerk-io-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-parcels-api-openapi.yml
- filename: clerk-io-privacy-api-openapi.yml
  format: yaml
  label: Clerk.io Privacy API
  slug: clerk-io-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-privacy-api-openapi.yml
- filename: clerk-io-product-data-api-openapi.yml
  format: yaml
  label: Clerk.io Product Data API
  slug: clerk-io-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-product-data-api-openapi.yml
- filename: clerk-io-recommendations-api-openapi.yml
  format: yaml
  label: Clerk.io Recommendations API
  slug: clerk-io-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-recommendations-api-openapi.yml
- filename: clerk-io-search-api-openapi.yml
  format: yaml
  label: Clerk.io Search API
  slug: clerk-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-search-api-openapi.yml
- filename: clerk-io-subscribers-api-openapi.yml
  format: yaml
  label: Clerk.io Subscribers API
  slug: clerk-io-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-subscribers-api-openapi.yml
- filename: clerk-io-tokens-api-openapi.yml
  format: yaml
  label: Clerk.io Tokens API
  slug: clerk-io-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-tokens-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Clerk Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clerk.io secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clerk.io
provider_slug: clerk-io
scheme_count: 3
schemes:
- in: query
  name: sec0
  note: The only securityScheme Clerk.io declares in its published OpenAPI. It covers the public key only.
  parameter: key
  role: public store identification
  sources:
  - openapi/clerk-io-openapi.yml
  type: apiKey
- in: body
  name: private_key
  note: Not modelled as an OpenAPI securityScheme by the provider - it appears as a required requestBody property on write operations (for example products-post, orders-post, customers-post). Recorded here because the documented auth model is incomplete without it.
  parameter: private_key
  role: store authentication for write and sensitive operations
  sources:
  - https://docs.clerk.io/docs/authentication
  - openapi/clerk-io-openapi.yml
  type: apiKey
- in: cookie
  name: jwt
  note: The /token/verify operation accepts a signed JWT as an httpOnly secure cookie, used to verify a visitor token rather than to authenticate an API caller.
  parameter: jwt
  role: visitor/session token verification
  scheme: bearer
  sources:
  - openapi/clerk-io-openapi.yml#token-verification
  type: http
slug: clerk-io-authentication
source_filename: clerk-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.clerk.io/docs/authentication\ndocs: https://docs.clerk.io/docs/authentication\nspec_source: openapi/clerk-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - body\n  model: dual-key\n  oauth2_flows: []\n  description: >-\n    Clerk.io authenticates at store level with a dual API key system. Every account has one public key and\n    one private key. The public key identifies the store, is safe to expose in browser-side calls, and is\n    sent as the `key` query parameter (GET) or `key` body field (POST/PATCH/DELETE). The private key\n    authenticates the store for sensitive operations - catalog writes, order and customer ingestion, and\n    sales statistics - and is sent as the `private_key` body field. Clerk.io's documentation requires SSL\n    whenever the private key is transmitted and warns that a holder of the private key can edit or delete\n    anything in the store.\nschemes:\n\
  - name: sec0\n  type: apiKey\n  in: query\n  parameter: key\n  role: public store identification\n  sources:\n  - openapi/clerk-io-openapi.yml\n  note: >-\n    The only securityScheme Clerk.io declares in its published OpenAPI. It covers the public key only.\n- name: private_key\n  type: apiKey\n  in: body\n  parameter: private_key\n  role: store authentication for write and sensitive operations\n  sources:\n  - https://docs.clerk.io/docs/authentication\n  - openapi/clerk-io-openapi.yml\n  note: >-\n    Not modelled as an OpenAPI securityScheme by the provider - it appears as a required requestBody\n    property on write operations (for example products-post, orders-post, customers-post). Recorded here\n    because the documented auth model is incomplete without it.\n- name: jwt\n  type: http\n  scheme: bearer\n  in: cookie\n  parameter: jwt\n  role: visitor/session token verification\n  sources:\n  - openapi/clerk-io-openapi.yml#token-verification\n  note: >-\n    The /token/verify operation\
  \ accepts a signed JWT as an httpOnly secure cookie, used to verify a\n    visitor token rather than to authenticate an API caller.\nrotation:\n  documented: false\n  note: No key-rotation or key-revocation procedure is published in the developer documentation.\ntransport:\n  tls_required: true\n  source: https://docs.clerk.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/authentication/clerk-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Artificial Intelligence
- Commerce
- E-Commerce
- Email Marketing
- Personalization
- Recommendations
- Search
---
