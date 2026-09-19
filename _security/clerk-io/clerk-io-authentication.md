---
anonymous_access: false
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
- filename: clerk-io-merchandising-api-openapi.yml
  format: yaml
  label: Clerk.io Merchandising API
  slug: clerk-io-merchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-merchandising-api-openapi.yml
- filename: clerk-io-privacy-api-openapi.yml
  format: yaml
  label: Clerk.io Privacy API
  slug: clerk-io-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-privacy-api-openapi.yml
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
- filename: clerk-io-categories-api-openapi.yml
  format: yaml
  label: Clerk.io Categories API
  slug: clerk-io-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-categories-api-openapi.yml
- filename: clerk-io-customers-api-openapi.yml
  format: yaml
  label: Clerk.io Customers API
  slug: clerk-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-customers-api-openapi.yml
- filename: clerk-io-customized-search-api-openapi.yml
  format: yaml
  label: Clerk.io Customized Search API
  slug: clerk-io-customized-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-customized-search-api-openapi.yml
- filename: clerk-io-log-api-openapi.yml
  format: yaml
  label: Clerk.io Log API
  slug: clerk-io-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-log-api-openapi.yml
- filename: clerk-io-orders-api-openapi.yml
  format: yaml
  label: Clerk.io Orders API
  slug: clerk-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-orders-api-openapi.yml
- filename: clerk-io-pages-api-openapi.yml
  format: yaml
  label: Clerk.io Pages API
  slug: clerk-io-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-pages-api-openapi.yml
- filename: clerk-io-product-api-openapi.yml
  format: yaml
  label: Clerk.io Product API
  slug: clerk-io-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-product-api-openapi.yml
- filename: clerk-io-products-api-openapi.yml
  format: yaml
  label: Clerk.io Products API
  slug: clerk-io-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-products-api-openapi.yml
- filename: clerk-io-redirects-api-openapi.yml
  format: yaml
  label: Clerk.io Redirects API
  slug: clerk-io-redirects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-redirects-api-openapi.yml
- filename: clerk-io-subscriber-api-openapi.yml
  format: yaml
  label: Clerk.io Subscriber API
  slug: clerk-io-subscriber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-subscriber-api-openapi.yml
- filename: clerk-io-synonyms-api-openapi.yml
  format: yaml
  label: Clerk.io Synonyms API
  slug: clerk-io-synonyms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-synonyms-api-openapi.yml
- filename: clerk-io-token-api-openapi.yml
  format: yaml
  label: Clerk.io Token API
  slug: clerk-io-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
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
