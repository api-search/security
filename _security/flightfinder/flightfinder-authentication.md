---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: FlightFinder Aviation Safety Data API
  slug: flightfinder-aviation-safety-data-api
  spec_type: OpenAPI
  url: https://himaxym.com/api/v1/data/openapi.json
auth_types:
- http
- none
description: 'FlightFinder''s Aviation Safety Data API is bearer-token only, with a documented keyless tier that answers every GET data endpoint with NO Authorization header at all. There is no OAuth, no OIDC, no mTLS and no query-string key: the API rejects ?api_key= outright. Key issuance is account-bound and happens over the same API.'
kind: authentication
layout: security
method: searched
name: Flightfinder Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlightFinder secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FlightFinder
provider_slug: flightfinder
scheme_count: 2
schemes:
- applies_to: all operations (declared as the top-level security requirement)
  description: API key as a bearer token. On the /keys management routes this is the account JWT instead — the API key itself cannot create or revoke keys.
  header: Authorization
  in: header
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/flightfinder-aviation-safety-data-openapi.json
  - https://himaxym.com/developers
  type: http
- applies_to: all GET data endpoints
  description: 'Documented anonymous tier. Every GET data endpoint answers with no Authorization header at 100 requests/day/IP. Confirmed live 2026-09-03: `curl ''https://himaxym.com/api/v1/data/events?limit=1''` returned HTTP 200 with real records and no credential.'
  name: keyless
  sources:
  - https://himaxym.com/developers
  type: none
slug: flightfinder-authentication
source_filename: flightfinder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: >-\n  https://himaxym.com/developers (Authentication + \"Get an API key\" sections) and\n  info.description / components.securitySchemes of\n  https://himaxym.com/api/v1/data/openapi.json. Live 401 bodies were observed on\n  2026-09-03 against https://himaxym.com/api/v1/data/ping and /events.\ndocs: https://himaxym.com/developers\ndescription: >-\n  FlightFinder's Aviation Safety Data API is bearer-token only, with a documented\n  keyless tier that answers every GET data endpoint with NO Authorization header at\n  all. There is no OAuth, no OIDC, no mTLS and no query-string key: the API rejects\n  ?api_key= outright. Key issuance is account-bound and happens over the same API.\nsummary:\n  types:\n  - http\n  - none\n  primary: http bearer\n  anonymous_tier: true\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    API key as a bearer token. On the /keys\
  \ management routes this is the account\n    JWT instead — the API key itself cannot create or revoke keys.\n  applies_to: all operations (declared as the top-level security requirement)\n  sources:\n  - openapi/flightfinder-aviation-safety-data-openapi.json\n  - https://himaxym.com/developers\n- name: keyless\n  type: none\n  description: >-\n    Documented anonymous tier. Every GET data endpoint answers with no Authorization\n    header at 100 requests/day/IP. Confirmed live 2026-09-03:\n    `curl 'https://himaxym.com/api/v1/data/events?limit=1'` returned HTTP 200 with\n    real records and no credential.\n  applies_to: all GET data endpoints\n  sources:\n  - https://himaxym.com/developers\ntoken_types:\n- name: API key\n  format: opaque bearer token\n  issued_by: POST /keys\n  issued_to: a himaxym.com account\n  shown: once — only a hash is stored server-side\n  max_active: 5 per account\n  revoke: DELETE /keys/{id}\n  propagation: a new key or a pro upgrade can take up to 5 minutes\
  \ to reach every worker\n- name: account JWT\n  format: JWT\n  used_for: the /keys management routes only (POST /keys, GET /keys, DELETE /keys/{id})\n  note: >-\n    An API key cannot create or revoke keys — the /keys routes require the account\n    token, and they return a different error envelope\n    ({\"success\":false,\"message\":\"Unauthorized\"}) than the data routes.\nprohibited:\n  query_string_key:\n    supported: false\n    status: 401\n    code: query_key_unsupported\n    reason_published: >-\n      \"query strings end up in access logs and browser history\" (OpenAPI\n      info.description and the /developers Authentication note)\n    observed: >-\n      GET https://himaxym.com/api/v1/data/events?limit=1&api_key=foo returned 401\n      {\"error\":{\"code\":\"query_key_unsupported\", ...}} on 2026-09-03\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  supported: false\n  note: >-\n    No scope surface exists. Access is tiered by plan (keyless / free key\
  \ / pro key),\n    not by scope, so scopes/ is intentionally absent rather than empty.\nerrors:\n- code: bad_key\n  status: 401\n  message: unknown or revoked API key\n  observed: true\n- code: query_key_unsupported\n  status: 401\n  message: 'passing the key as ?api_key= is no longer supported — send it as an Authorization: Bearer header'\n  observed: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightfinder/refs/heads/main/authentication/flightfinder-authentication.yml
summary_line: http/none · 2 schemes
tags:
- Aviation
- Aviation Safety
- Accident Data
- Open Data
- Public Domain
- Transportation
- Government Data
- Research
- Reference Data
- Agent Ready
---
