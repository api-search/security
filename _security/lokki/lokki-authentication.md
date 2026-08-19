---
api_key_in:
- header
api_specs:
- filename: lokki-external-api-openapi.json
  format: json
  label: Lokki External API
  slug: lokki-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/openapi/lokki-external-api-openapi.json
- filename: lokki-dashboard-api-openapi.json
  format: json
  label: Lokki Dashboard API
  slug: lokki-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/openapi/lokki-dashboard-api-openapi.json
auth_types:
- apiKey
description: 'Lokki authenticates with a single long-lived API key (an "Access Token") in a request header. There is no OAuth, no OIDC, no token endpoint, and no self-serve key issuance: keys are handed out by a Lokki representative as part of a partnership agreement, separately for staging and production, and are scoped at three levels.'
kind: authentication
layout: security
method: searched
name: Lokki Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lokki secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lokki
provider_slug: lokki
scheme_count: 2
schemes:
- applies_to: Lokki External API (partner surface)
  documented_example: 'GET /v2/external/stores

    Host: prod.api.eu-west-3.lokki.rent

    x-api-key: YOUR_ACCESS_TOKEN

    '
  in: header
  method: searched
  name: x-api-key
  parameter: x-api-key
  source: https://docs.getlokki.com/api-reference/authentication
  type: apiKey
- applies_to: Lokki Dashboard API (internal) — and declared as the security scheme in BOTH published specs
  bearer_format: JWT
  in: header
  method: derived
  name: x-access-token
  parameter: x-access-token
  scheme: bearer
  sources:
  - openapi/lokki-dashboard-api-openapi.json
  - openapi/lokki-external-api-openapi.json
  type: apiKey
slug: lokki-authentication
source_filename: lokki-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: >-\n  https://docs.getlokki.com/api-reference/authentication (documented), plus the securitySchemes\n  derived from openapi/lokki-external-api-openapi.json and\n  openapi/lokki-dashboard-api-openapi.json by 0-working/derive-authentication.py, and a live\n  unauthenticated probe of https://prod.api.eu-west-3.lokki.rent/v2/external/verticales on 2026-08-17.\ndescription: >-\n  Lokki authenticates with a single long-lived API key (an \"Access Token\") in a request header. There is\n  no OAuth, no OIDC, no token endpoint, and no self-serve key issuance: keys are handed out by a Lokki\n  representative as part of a partnership agreement, separately for staging and production, and are\n  scoped at three levels.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  oidc: false\n  mutual_tls: false\n  self_serve_keys: false\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n\
  \  applies_to: Lokki External API (partner surface)\n  method: searched\n  source: https://docs.getlokki.com/api-reference/authentication\n  documented_example: |\n    GET /v2/external/stores\n    Host: prod.api.eu-west-3.lokki.rent\n    x-api-key: YOUR_ACCESS_TOKEN\n- name: x-access-token\n  type: apiKey\n  in: header\n  parameter: x-access-token\n  scheme: bearer\n  bearer_format: JWT\n  applies_to: Lokki Dashboard API (internal) — and declared as the security scheme in BOTH published specs\n  method: derived\n  sources:\n  - openapi/lokki-dashboard-api-openapi.json\n  - openapi/lokki-external-api-openapi.json\nheader_discrepancy:\n  documented: x-api-key\n  in_spec: x-access-token\n  note: >-\n    The published partner OpenAPI declares its only securityScheme as `x-access-token`, but the\n    authentication page, the getting-started page and Lokki's own published Agent Skill all say\n    `x-api-key` — and the Agent Skill explicitly lists \"Wrong header name: must be x-api-key, not\n\
  \    x-api-token or Authorization. Incorrect header returns 401\" as a common gotcha. x-access-token is\n    the header the internal Dashboard API uses for its JWT, so the partner spec appears to have\n    inherited the internal scheme. A client generated from the spec would send the wrong header. Not\n    resolved here — only Lokki can say which is authoritative. Recorded also in\n    conventions/lokki-conventions.yml.\nkey_format:\n  staging_prefix: lokki_sk_test_\n  production_prefix: lokki_sk_live_\n  environment_bound: true\n  statement: A token generated for Staging will not work on Production, and vice-versa.\nscopes:\n  model: three-level key scoping (not OAuth scopes — no scope parameter, no consent screen)\n  levels:\n  - {level: domain, description: 'access to specific data sets, e.g. stores, items'}\n  - {level: action, description: 'permission to perform specific actions: read, write'}\n  - {level: route, description: 'access to specific HTTP methods, e.g. GET, POST'}\n  assignment:\
  \ Set by Lokki according to the partnership agreement; a partner cannot self-modify scope.\n  failure_mode: 403 Forbidden when the key lacks the required scope for an endpoint.\n  note: >-\n    No scopes/ artifact is published for Lokki because these are API-key permissions, not OAuth2\n    scopes; 0-working/derive-oauth-scopes.py found no oauth2 securityScheme to derive from.\nissuance:\n  self_serve: false\n  process: Contact your Lokki representative; they guide the partnership process and provide credentials for both environments.\n  rotation: On request — \"if you suspect a token has been compromised, contact your Lokki representative immediately to revoke it and issue a new one.\"\n  programmatic_rotation: false\n  expiry: not published\npublished_guidance:\n- Treat the access token like a password; never expose it in client-side code or public repositories.\n- Store tokens in environment variables or a secret-management system.\nobserved_behaviour:\n  probe: GET https://prod.api.eu-west-3.lokki.rent/v2/external/verticales\
  \ (no credentials)\n  http_status: 403\n  body: '{\"statusCode\":403,\"message\":\"Forbidden resource\",\"error\":\"Forbidden\"}'\n  date: '2026-08-17'\n  note: >-\n    An anonymous call returns 403, not the 401 the docs describe for a missing token. Both codes are\n    reachable — see errors/lokki-problem-types.yml.\ndocs: https://docs.getlokki.com/api-reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lokki/refs/heads/main/authentication/lokki-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Climate Tech
- Circular Economy
- Rental
- Equipment Rental
- Bike Rental
- Marketplace
- Booking
- Reservations
- Inventory
- Catalog
- Pricing
- Availability
- Mobility
- Outdoor Recreation
- Point of Sale
- SaaS
- France
- MCP
- Agents
- Agent Skills
---
