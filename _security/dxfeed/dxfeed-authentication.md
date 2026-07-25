---
api_key_in: []
api_specs:
- filename: dxfeed-dxlink-asyncapi.yml
  format: yaml
  label: dxFeed dxLink WebSocket API
  slug: dxfeed-dxlink-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dxfeed/refs/heads/main/asyncapi/dxfeed-dxlink-asyncapi.yml
- filename: dxfeed-fundamentals-openapi.json
  format: json
  label: dxFeed Fundamentals API
  slug: dxfeed-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dxfeed/refs/heads/main/openapi/dxfeed-fundamentals-openapi.json
auth_types:
- http-basic (login/password credentials)
- dxLink AUTH token (protocol message)
description: ''
kind: authentication
layout: security
method: searched
name: Dxfeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: dxFeed secures its APIs with http-basic (login/password credentials) and dxLink AUTH token (protocol message) across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: dxFeed
provider_slug: dxfeed
scheme_count: 3
schemes:
- description: Login/password credentials with per-service entitlements for REST webservice, IPF web service (tools.dxfeed.com/ipf returns 401 without them), Fundamentals production, and historical/tick extraction.
  name: credentials
  scheme: basic
  sources:
  - https://kb.dxfeed.com/en/data-model/reference-data/ipf-webservice.html
  - 'live probe: tools.dxfeed.com/ipf HTTP 401'
  type: http
- description: 'dxLink WebSocket protocol authentication: after SETUP, the server sends AUTH_STATE UNAUTHORIZED and the client sends an AUTH message carrying a token; the server replies AUTH_STATE AUTHORIZED. Token issuance is part of dxFeed onboarding; the demo server does not require auth.'
  name: dxlink-auth
  sources:
  - asyncapi/dxfeed-dxlink-asyncapi.yml
  type: protocol-message
- description: The Fundamentals OpenAPI (tools.dxfeed.com/fs/v3/api-docs) declares no securitySchemes; entitlements are enforced out-of-band (403 responses declared on every operation; live production endpoints are credential-gated).
  name: fundamentals-openapi
  sources:
  - openapi/dxfeed-fundamentals-openapi.json
  type: none-declared
slug: dxfeed-authentication
source_filename: dxfeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://kb.dxfeed.com/en/getting-started.html\nsource: kb.dxfeed.com docs + asyncapi/dxfeed-dxlink-asyncapi.yml + live probes\nsummary:\n  types:\n  - http-basic (login/password credentials)\n  - dxLink AUTH token (protocol message)\n  self_serve: false\n  note: No OAuth, no self-serve API keys. Production credentials (endpoint URLs, login, password) plus\n    per-service entitlements are issued during sales onboarding. Public demo endpoints (demo.dxfeed.com\n    REST webservice, wss://demo.dxfeed.com/dxlink-ws) require no credentials and serve delayed data.\nschemes:\n- name: credentials\n  type: http\n  scheme: basic\n  description: Login/password credentials with per-service entitlements for REST webservice, IPF web service\n    (tools.dxfeed.com/ipf returns 401 without them), Fundamentals production, and historical/tick extraction.\n  sources:\n  - https://kb.dxfeed.com/en/data-model/reference-data/ipf-webservice.html\n \
  \ - 'live probe: tools.dxfeed.com/ipf HTTP 401'\n- name: dxlink-auth\n  type: protocol-message\n  description: 'dxLink WebSocket protocol authentication: after SETUP, the server sends AUTH_STATE UNAUTHORIZED\n    and the client sends an AUTH message carrying a token; the server replies AUTH_STATE AUTHORIZED. Token\n    issuance is part of dxFeed onboarding; the demo server does not require auth.'\n  sources:\n  - asyncapi/dxfeed-dxlink-asyncapi.yml\n- name: fundamentals-openapi\n  type: none-declared\n  description: The Fundamentals OpenAPI (tools.dxfeed.com/fs/v3/api-docs) declares no securitySchemes;\n    entitlements are enforced out-of-band (403 responses declared on every operation; live production\n    endpoints are credential-gated).\n  sources:\n  - openapi/dxfeed-fundamentals-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dxfeed/refs/heads/main/authentication/dxfeed-authentication.yml
summary_line: http-basic (login/password credentials)/dxLink AUTH token (protocol message) · 3 schemes
tags:
- Financial
- Market Data
- Real-Time
- Historical Data
- Equities
- Options
- Futures
- Crypto
- Reference Data
- Fundamentals
---
