---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Byrd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Byrd secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Byrd
provider_slug: byrd
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'All byrd API calls require an Authorization header carrying a JWT bearer token: `Authorization: Bearer <JWT TOKEN>`. Tokens are obtained by posting credentials to the login endpoint and are valid for up to 7 days by default (configurable via the `validity` parameter, in seconds). Tokens should be cached and reused until expiry rather than re-fetched per request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developers.getbyrd.com/docs/authentication
  type: http
slug: byrd-authentication
source_filename: byrd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.getbyrd.com/docs/authentication\ndocs: https://developers.getbyrd.com/docs/authentication\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      All byrd API calls require an Authorization header carrying a JWT bearer\n      token: `Authorization: Bearer <JWT TOKEN>`. Tokens are obtained by posting\n      credentials to the login endpoint and are valid for up to 7 days by default\n      (configurable via the `validity` parameter, in seconds). Tokens should be\n      cached and reused until expiry rather than re-fetched per request.\n    sources: [https://developers.getbyrd.com/docs/authentication]\ntoken_endpoints:\n  login: https://api.getbyrd.com/v2/login          # POST — exchange credentials for JWT\n  refresh: https://api.getbyrd.com/v2/refresh_token\
  \ # POST — mint a fresh access token\nnotes:\n  - >-\n    A required User-Agent header must identify the caller in the form\n    \"<company-registered-in-byrd> (tech-contact-email) - <optional integration version>\".\n  - Login endpoint is rate limited to 5 calls per minute per IP or User-Agent.\n  - HTTPS with TLS v1.2 or above is required on every endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/authentication/byrd-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- E-Commerce
- Fulfillment
- Logistics
- 3PL
- Shipping
- Warehousing
- Order Management
- Inventory
- Returns
- Supply Chain
---
