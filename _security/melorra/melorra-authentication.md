---
api_key_in: []
api_specs:
- filename: melorra-discovery-api-openapi.yml
  format: yaml
  label: Melorra Discovery API
  slug: melorra-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/openapi/melorra-discovery-api-openapi.yml
- filename: melorra-products-api-openapi.yml
  format: yaml
  label: Melorra Products API
  slug: melorra-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/openapi/melorra-products-api-openapi.yml
- filename: melorra-recommendations-api-openapi.yml
  format: yaml
  label: Melorra Recommendations API
  slug: melorra-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/openapi/melorra-recommendations-api-openapi.yml
- filename: melorra-silver-api-openapi.yml
  format: yaml
  label: Melorra Silver API
  slug: melorra-silver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/openapi/melorra-silver-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Melorra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Melorra declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Melorra
provider_slug: melorra
scheme_count: 0
schemes: []
slug: melorra-authentication
source_filename: melorra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  live unauthenticated requests to https://services-catalog.melorra.com/api/* on 2026-08-25, plus\n  Melorra's published /.well-known/api-catalog which documents no authentication requirement.\nsummary: >-\n  The Melorra Catalog API requires NO authentication. Every documented and advertised endpoint\n  returned 200 to an anonymous GET with no API key, token, cookie or signed header. The OpenAPI\n  description carries no securitySchemes because the provider imposes none — this is an absence\n  that was verified, not one that was assumed.\nschemes: []\nmodel:\n  type: none\n  anonymous_access: true\n  credentials_required: false\n  verified_anonymous:\n  - url: https://services-catalog.melorra.com/api/product/products/?page=1\n    status: 200\n  - url: https://services-catalog.melorra.com/api/product/products/232484/\n    status: 200\n  - url: https://services-catalog.melorra.com/api/product/product/\n    status: 200\n  -\
  \ url: https://services-catalog.melorra.com/api/product/similar/\n    status: 200\noauth:\n  supported: false\n  discovery_probed:\n  - url: https://services-catalog.melorra.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://services-catalog.melorra.com/.well-known/openid-configuration\n    status: 404\nnotes:\n- >-\n  There is no developer signup, key issuance, or plan gate in front of this API. The consumer-facing\n  https://www.melorra.com/sign-in/ page is a retail shopper account, not an API credential surface.\n- >-\n  Because access is anonymous, there is no per-key attribution and therefore no per-key rate limit\n  or quota an agent can reason about. See rate-limits/melorra-rate-limits.yml.\n- >-\n  The response headers set X-Frame-Options DENY, X-Content-Type-Options nosniff, Referrer-Policy\n  same-origin and Cross-Origin-Opener-Policy same-origin, and Vary includes Origin — but no CORS\n  Access-Control-Allow-Origin was returned to an anonymous cross-origin-less\
  \ request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/authentication/melorra-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Jewellery
- Retail
- E-Commerce
- Product Catalog
- Direct to Consumer
- Fashion
- India
---
