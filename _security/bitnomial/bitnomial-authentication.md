---
api_key_in:
- header
api_specs:
- filename: bitnomial-market-data-asyncapi.yml
  format: yaml
  label: Bitnomial Market Data WebSocket API
  slug: bitnomial-market-data-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitnomial/refs/heads/main/asyncapi/bitnomial-market-data-asyncapi.yml
auth_types:
- hmac-signed-api-key
description: ''
kind: authentication
layout: security
method: searched
name: Bitnomial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitnomial secures its APIs with hmac-signed-api-key across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitnomial
provider_slug: bitnomial
scheme_count: 1
schemes:
- credential_model: A ConnectionId + AuthToken pair provisioned in the customer portal. A connection grants access to data for all accounts associated with it.
  headers:
  - description: Hex-encoded ConnectionId identifying the API connection.
    name: BTNL-CONNECTION-ID
  - description: ISO 8601 timestamp (YYYY-MM-DDTHH:MM:SS.SSSZ). Must be within 30 seconds of exchange time or the request is rejected.
    name: BTNL-AUTH-TIMESTAMP
  - description: Base64-encoded HMAC-SHA256 signature. The signed string is method + requestPath + queryString + headers + body, using the ConnectionId's hex-encoded AuthToken as the HMAC secret.
    name: BTNL-SIGNATURE
  in: header
  name: btnl-signature
  scheme: hmac-sha256-request-signature
  sources:
  - docs
  type: apiKey
slug: bitnomial-authentication
source_filename: bitnomial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bitnomial.com/exchange/docs/api/rest/authentication/\ndocs: https://bitnomial.com/exchange/docs/api/rest/authentication/\nsummary:\n  types: [hmac-signed-api-key]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    No OAuth / OpenID Connect. Private REST endpoints are authenticated with a\n    per-request HMAC-SHA256 request signature keyed on a symmetric AuthToken\n    issued alongside a ConnectionId in the customer portal. There is therefore\n    no OAuth scope surface (scopes/ is intentionally omitted).\nschemes:\n  - name: btnl-signature\n    type: apiKey\n    scheme: hmac-sha256-request-signature\n    in: header\n    headers:\n      - name: BTNL-CONNECTION-ID\n        description: Hex-encoded ConnectionId identifying the API connection.\n      - name: BTNL-AUTH-TIMESTAMP\n        description: >-\n          ISO 8601 timestamp (YYYY-MM-DDTHH:MM:SS.SSSZ). Must be within 30\n          seconds of exchange\
  \ time or the request is rejected.\n      - name: BTNL-SIGNATURE\n        description: >-\n          Base64-encoded HMAC-SHA256 signature. The signed string is\n          method + requestPath + queryString + headers + body, using the\n          ConnectionId's hex-encoded AuthToken as the HMAC secret.\n    credential_model: >-\n      A ConnectionId + AuthToken pair provisioned in the customer portal. A\n      connection grants access to data for all accounts associated with it.\n    sources: [docs]\npublic_endpoints:\n  - path: /product/data/\n    note: Product data is publicly available (no signature required).\n  - path: /funding-rates\n    note: Perpetual funding rates are publicly available.\n  - path: /market-stats\n    note: Market statistics are publicly available.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitnomial/refs/heads/main/authentication/bitnomial-authentication.yml
summary_line: hmac-signed-api-key · 1 scheme
tags:
- Company
- Fintech
- Cryptocurrency
- Derivatives
- Exchange
- Trading
- Market Data
- Futures
- Options
- CFTC Regulated
---
