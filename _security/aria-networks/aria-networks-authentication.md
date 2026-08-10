---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Aria Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aria Networks declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aria Networks
provider_slug: aria-networks
scheme_count: 1
schemes:
- bearerFormat: JWT
  evidence: 'GET https://api.arianetworks.com/v1/fabrics with "Authorization: Bearer <invalid>" returns HTTP 401 {"type":"invalid_request_error","message":"Invalid Compact JWS", ...}. The "Invalid Compact JWS" message confirms the bearer credential is parsed as a compact-serialized JWS (JWT). Without the header the same request returns "Authentication required".'
  header: Authorization
  in: header
  name: bearerAuth
  observed: '2026-08-06'
  scheme: bearer
  type: http
slug: aria-networks-authentication
source_filename: aria-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://api.arianetworks.com/v1/fabrics\nnote: >-\n  Aria Networks publishes no OpenAPI and no public authentication documentation —\n  docs.arianetworks.com redirects every path to /login. This profile is therefore\n  derived from what the live API itself reveals to an anonymous caller, not from a\n  provider-published auth page. Every value below is backed by an observed response.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  evidence: >-\n    GET https://api.arianetworks.com/v1/fabrics with\n    \"Authorization: Bearer <invalid>\" returns HTTP 401\n    {\"type\":\"invalid_request_error\",\"message\":\"Invalid Compact JWS\", ...}. The\n    \"Invalid Compact JWS\" message confirms the bearer credential is parsed as a\n    compact-serialized JWS (JWT). Without the header the same request returns\n    \"Authentication required\".\n  observed: '2026-08-06'\n\
  challenge:\n  www_authenticate: false\n  note: >-\n    The API returns 401 with a JSON body but does NOT emit a WWW-Authenticate\n    response header, so an agent cannot discover the scheme from the challenge\n    alone.\ncors:\n  allow_headers:\n  - Content-Type\n  - Authorization\n  allow_methods:\n  - GET\n  - POST\n  - PUT\n  - DELETE\n  - PATCH\n  - OPTIONS\n  max_age: 86400\n  evidence: OPTIONS https://api.arianetworks.com/v1/fabrics\nkey_management:\n  resource: /v1/api-keys\n  status: gated\n  note: >-\n    The unauthenticated root index at https://api.arianetworks.com/ advertises an\n    \"apiKeys\": \"/v1/api-keys\" resource and an \"auth\": \"/v1/auth\" resource, so\n    programmatic key issuance exists. Both return 401 anonymously and neither is\n    documented publicly, so the credential lifecycle (issuance, rotation, scoping)\n    could not be observed.\noauth2: false\nopenid_connect: false\nscopes_published: false\ndocs: null\ndocs_note: >-\n  https://docs.arianetworks.com/\
  \ HTTP 302 -> /login for every path. No public\n  authentication reference exists.\nx-evidence:\n- url: https://api.arianetworks.com/v1/fabrics\n  http_status: 401\n  fetched: '2026-08-06'\n- url: https://api.arianetworks.com/v1/health\n  http_status: 200\n  fetched: '2026-08-06'\n- url: https://docs.arianetworks.com/\n  http_status: 302\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aria-networks/refs/heads/main/authentication/aria-networks-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Networking
- Data Center
- Artificial Intelligence
- Infrastructure
- Telemetry
- Observability
- Ethernet
- Hardware
---
