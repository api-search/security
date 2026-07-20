---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Falcon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Falcon secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Falcon
provider_slug: falcon
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'JWT access token returned by POST /api/v1/login, passed as "Authorization: Bearer <token>" on subsequent requests. Token lifetime ~10 minutes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.falconfs.com/reference/authentication
  type: http
- description: Per-tenant routing header required on every request.
  in: header
  name: x-tenant-id
  sources:
  - https://docs.falconfs.com/reference/authentication
  type: apiKey
- description: Client id and client secret headers used only against the login endpoint to mint the JWT access token.
  in: header
  name: x-client-id + clientSecret
  sources:
  - https://docs.falconfs.com/reference/authentication
  type: apiKey
slug: falcon-authentication
source_filename: falcon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.falconfs.com/reference/authentication\ndocs: https://docs.falconfs.com/reference/authentication\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  bearer_format: JWT\n  notes: >-\n    Falcon uses a two-step credential model. A client authenticates with a client id\n    and client secret to mint a short-lived JWT access token, then presents that token\n    as an HTTP bearer Authorization header on all subsequent calls. Requests are\n    additionally scoped to a tenant via an x-tenant-id header, and request/response\n    bodies are AES-encrypted with a pre-shared symmetric key. There is no documented\n    public OAuth authorization/scope surface; the underlying identity provider is a\n    Keycloak realm (token issuer path .../idam/realms/<tenant>).\ngateway_url: https://credituat.falconfs.com/\nlogin:\n  operation: POST /api/v1/login\n  request_headers:\n    - name: x-client-id\n\
  \      required: true\n      description: Client identifier issued by Falcon.\n    - name: clientSecret\n      required: true\n      description: Client secret key issued by Falcon.\n    - name: x-tenant-id\n      required: true\n      description: Tenant identifier (for example, falcon or kvb).\n  returns: JWT access token (token_type Bearer), expires in ~10 minutes (exp is Unix epoch).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      JWT access token returned by POST /api/v1/login, passed as\n      \"Authorization: Bearer <token>\" on subsequent requests. Token lifetime ~10 minutes.\n    sources: [https://docs.falconfs.com/reference/authentication]\n  - name: tenantHeader\n    type: apiKey\n    in: header\n    name: x-tenant-id\n    description: Per-tenant routing header required on every request.\n    sources: [https://docs.falconfs.com/reference/authentication]\n  - name: clientCredentials\n    type: apiKey\n   \
  \ in: header\n    name: x-client-id + clientSecret\n    description: >-\n      Client id and client secret headers used only against the login endpoint to\n      mint the JWT access token.\n    sources: [https://docs.falconfs.com/reference/authentication]\nencryption:\n  scheme: AES (symmetric, pre-shared key)\n  applies_to: [request body, response body]\n  note: >-\n    Non-production keys are shared by Falcon; in production the bank shares the key and\n    Falcon configures it. Encrypted payload is sent as a Base64 string in place of the\n    JSON body; headers remain plaintext.\nrequest_headers:\n  - {name: Authorization, description: \"Bearer JWT access token.\"}\n  - {name: x-tenant-id, description: \"Tenant identifier.\"}\n  - {name: Content-Type, description: \"application/json.\"}\nresponse_headers:\n  - {name: x-trace-id, description: \"Unique per-request trace identifier for support/troubleshooting.\"}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/falcon/refs/heads/main/authentication/falcon-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Infrastructure
- Financial Services
- Banking
- Payments
- Credit Cards
- Embedded Finance
- Fintech
- Card Issuing
- Lending
- Banking as a Service
- India
---
