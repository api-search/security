---
api_key_in:
- header
- query
api_specs:
- filename: openapi.json
  format: json
  label: TheCarApi REST API
  slug: thecarapi-rest-api
  spec_type: OpenAPI
  url: https://thecarapi.com/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Thecarapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheCarApi secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TheCarApi
provider_slug: thecarapi
scheme_count: 3
schemes:
- description: Recommended for server-to-server calls.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  recommended: true
  sources:
  - openapi/thecarapi-openapi.json
  - https://thecarapi.com/docs/authentication
  type: apiKey
- description: 'Authorization: Bearer <key>. Documented as equivalent to X-API-Key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thecarapi-openapi.json
  - https://thecarapi.com/docs/authentication
  type: http
- default_enabled: false
  description: ?api_key=<key>. Disabled by default and enabled per key on request. The provider warns that keys in URLs end up in logs and referrers. Not declared in the OpenAPI securitySchemes.
  documented_only: true
  in: query
  name: queryApiKey
  parameter: api_key
  sources:
  - https://thecarapi.com/docs/authentication
  type: apiKey
slug: thecarapi-authentication
source_filename: thecarapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://thecarapi.com/docs/authentication\ndocs: https://thecarapi.com/docs/authentication\nspec_source: openapi/thecarapi-openapi.json\nsummary:\n  model: api-key\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - header\n    - query\n  note: >-\n    Every endpoint except the two unauthenticated liveness probes (/api/health/live and\n    /api/health/ready) requires an API key. The three presentation methods are interchangeable;\n    the provider recommends the X-API-Key header for server-to-server calls.\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    recommended: true\n    description: Recommended for server-to-server calls.\n    sources:\n      - openapi/thecarapi-openapi.json\n      - https://thecarapi.com/docs/authentication\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description:\
  \ 'Authorization: Bearer <key>. Documented as equivalent to X-API-Key.'\n    sources:\n      - openapi/thecarapi-openapi.json\n      - https://thecarapi.com/docs/authentication\n  - name: queryApiKey\n    type: apiKey\n    in: query\n    parameter: api_key\n    documented_only: true\n    default_enabled: false\n    description: >-\n      ?api_key=<key>. Disabled by default and enabled per key on request. The provider warns that\n      keys in URLs end up in logs and referrers. Not declared in the OpenAPI securitySchemes.\n    sources:\n      - https://thecarapi.com/docs/authentication\nunauthenticated_endpoints:\n  - operationId: get_api_health_live\n    path: /api/health/live\n    note: Process liveness probe. No key, no quota.\n  - operationId: get_api_health_ready\n    path: /api/health/ready\n    note: Readiness probe. No key, no quota. 503 while the data layer is unreachable.\nkey_restrictions:\n  - restriction: ip_or_cidr_allowlist\n    effect_when_violated: '403'\n  - restriction:\
  \ origin_allowlist\n    effect_when_violated: '403'\n    note: Browser requests from other origins.\n  - restriction: expiry_date\n    effect_when_violated: '401'\n  - restriction: status_revoked_or_suspended\n    effect_when_violated: '403'\n  - restriction: scope_set\n    effect_when_violated: '403'\n    body: '{\"success\": false, \"error\": \"API key is not authorized for this route\"}'\n    note: >-\n      No machine-readable error code in the body — the provider tells clients to branch on the\n      status code, not the message text.\nbrute_force_lockout:\n  trigger: five failed authentication attempts from one IP\n  effect: every subsequent request from that address returns 429 for 15 minutes, including requests carrying a valid key\n  reset: a successful authentication clears the counter\n  source: https://thecarapi.com/docs/authentication\nclient_side_guidance: >-\n  The provider explicitly warns against shipping a full-access key to a browser or mobile app, and\n  recommends\
  \ a separate key with an origin allowlist and minimum scopes, or a backend proxy.\nscopes_artifact: scopes/thecarapi-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecarapi/refs/heads/main/authentication/thecarapi-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Automotive
- Vehicle Data
- Car Auctions
- Used Cars
- Vehicle Inventory
- Classifieds
- Market Intelligence
- Pricing
- VIN
- Image CDN
- Europe
- Korea
- Japan Auctions
---
