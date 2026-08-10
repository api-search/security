---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Claim Genius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Claim Genius secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Claim Genius
provider_slug: claim-genius
scheme_count: 1
schemes:
- bearerFormat: JWT
  credentials:
  - API ID
  - API secret
  description: JWT-based authentication. The provider states each integrator is issued a unique API ID and API secret, which are exchanged for a JWT session token; a single API token then reaches all Genius products and outputs.
  name: jwtBearer
  scheme: bearer
  sources:
  - https://claimgenius.com/geniusapi
  token_endpoint: /api/auth/token
  type: http
slug: claim-genius-authentication
source_filename: claim-genius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://claimgenius.com/geniusapi\ndocs: https://claimgenius.com/geniusapi\nnote: >-\n  Derived from the provider's own public GeniusAPI product page, not from a machine-readable spec.\n  Claim Genius publishes no OpenAPI, no reference documentation and no security scheme definition at a\n  public URL, so the fields below record what the company states about its auth model, at the level of\n  detail it states it. Full scheme detail (header name, token TTL, refresh behavior, error shapes)\n  requires developer access, which is requested by email.\nsummary:\n  types:\n  - http\n  bearer_formats:\n  - JWT\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: jwtBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    JWT-based authentication. The provider states each integrator is issued a unique API ID and API\n    secret, which are exchanged\
  \ for a JWT session token; a single API token then reaches all Genius\n    products and outputs.\n  token_endpoint: /api/auth/token\n  credentials:\n  - API ID\n  - API secret\n  sources:\n  - https://claimgenius.com/geniusapi\ncredential_issuance:\n  self_serve: false\n  channel: email\n  contact: contactus@claimgenius.com\n  statement: >-\n    \"Contact us at contactus@claimgenius.com to request developer access and documentation.\"\n  cta: Request API Access\nx-evidence:\n- url: https://claimgenius.com/geniusapi\n  http_status: 200\n  fetched: '2026-08-09'\n  note: >-\n    Page is a client-rendered React route; the served HTML is an empty shell. Copy was read from the\n    published route bundle https://claimgenius.com/assets/GeniusApiPage-2efvqe5o.js (HTTP 200).\n- url: https://claimgenius.com/assets/GeniusApiPage-2efvqe5o.js\n  http_status: 200\n  fetched: '2026-08-09'\n- url: https://api.claimgenius.com/api/auth/token\n  http_status: 404\n  fetched: '2026-08-09'\n  note: nginx 404\
  \ — the documented token endpoint is not served at the api. host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claim-genius/refs/heads/main/authentication/claim-genius-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurance Claims
- Insurance Underwriting
- Artificial Intelligence
- Computer Vision
- Vehicle Inspection
- Automotive
- Claims Automation
- Damage Assessment
- InsurTech
---
