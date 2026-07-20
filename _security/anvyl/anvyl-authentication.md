---
api_key_in: []
auth_types:
- http
description: 'No public OpenAPI/Swagger document is exposed by Anvyl (developer docs are served as a gated Stoplight SPA), so the auth model here is captured from observed live behavior rather than derived from a spec. Unauthenticated requests to the REST API return HTTP 401 with {"error":"Unauthorized"}. A request carrying an Authorization: Bearer <token> header passes the auth gate (the same route then returns 404 for an unknown token context rather than 401), whereas an X-API-Key header does not (still 401) — indicating the API authenticates with a bearer token in the standard Authorization header.'
kind: authentication
layout: security
method: searched
name: Anvyl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anvyl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anvyl
provider_slug: anvyl
scheme_count: 1
schemes:
- description: 'Bearer token supplied in the Authorization header (Authorization: Bearer <token>). Tokens are provisioned via the Anvyl platform''s API access feature; see the developer docs for issuance.'
  evidence:
  - GET https://api.anvyl.com/api/v1 without auth -> 401 {"error":"Unauthorized"}
  - 'GET https://api.anvyl.com/api/v1/purchase_orders with Authorization: Bearer <bogus> -> 404 (past the 401 gate)'
  - 'GET https://api.anvyl.com/api/v1/purchase_orders with X-API-Key: <bogus> -> 401 (header not honored)'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - live probe
  type: http
slug: anvyl-authentication
source_filename: anvyl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  Live probe of https://api.anvyl.com/api/v1 plus the Anvyl developer\n  documentation at https://anvyl.stoplight.io/docs/anvyl-api\ndescription: >-\n  No public OpenAPI/Swagger document is exposed by Anvyl (developer docs are\n  served as a gated Stoplight SPA), so the auth model here is captured from\n  observed live behavior rather than derived from a spec. Unauthenticated\n  requests to the REST API return HTTP 401 with {\"error\":\"Unauthorized\"}. A\n  request carrying an Authorization: Bearer <token> header passes the auth gate\n  (the same route then returns 404 for an unknown token context rather than\n  401), whereas an X-API-Key header does not (still 401) — indicating the API\n  authenticates with a bearer token in the standard Authorization header.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n\
  \    in: header\n    header: Authorization\n    description: >-\n      Bearer token supplied in the Authorization header\n      (Authorization: Bearer <token>). Tokens are provisioned via the Anvyl\n      platform's API access feature; see the developer docs for issuance.\n    evidence:\n      - \"GET https://api.anvyl.com/api/v1 without auth -> 401 {\\\"error\\\":\\\"Unauthorized\\\"}\"\n      - \"GET https://api.anvyl.com/api/v1/purchase_orders with Authorization: Bearer <bogus> -> 404 (past the 401 gate)\"\n      - \"GET https://api.anvyl.com/api/v1/purchase_orders with X-API-Key: <bogus> -> 401 (header not honored)\"\n    sources:\n      - live probe\ndocs: https://anvyl.stoplight.io/docs/anvyl-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anvyl/refs/heads/main/authentication/anvyl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Supply Chain
- Procurement
- Purchase Orders
- Manufacturing
- Production Management
---
