---
api_key_in:
- body
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Carserv Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarServ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CarServ
provider_slug: carserv
scheme_count: 1
schemes:
- applied_to: all Public API resource requests
  bearerFormat: JWT
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://github.com/CarServ/public_api_client
  type: http
  value_format: Bearer <jwt>
slug: carserv-authentication
source_filename: carserv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: >-\n  https://github.com/CarServ/public_api_client —\n  lib/carserv/public_api/client/authenticator.rb,\n  lib/carserv/public_api/client/config.rb,\n  lib/carserv/public_api/client/resources/base.rb\nnotes: >-\n  Derived from the first-party Ruby client, not from an OpenAPI definition —\n  CarServ never published a machine-readable spec and the developer site is gone.\n  The model is a two-legged key/secret token exchange that returns a JWT, which is\n  then sent as a bearer token on every JSON:API request. Not OAuth 2.0: there is no\n  authorization endpoint, no scopes, no refresh token and no grant_type parameter,\n  so no scopes/ artifact is produced.\nsummary:\n  types:\n  - http\n  bearer_format: JWT\n  api_key_in:\n  - body\n  oauth2_flows: []\n  scopes_supported: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  value_format: 'Bearer <jwt>'\n\
  \  applied_to: all Public API resource requests\n  sources:\n  - https://github.com/CarServ/public_api_client\ntoken_exchange:\n  method: POST\n  path: /public/api/v2/access_token.json\n  request_content_type: application/json\n  request_body_fields:\n  - name: key\n    description: CarServ API key issued to the integrating account\n  - name: secret\n    description: CarServ API secret paired with the key\n  response_field: jwt\n  description: >-\n    Credentials are exchanged for a JWT which the client caches (the reference\n    client caches it in Redis under access_token_<api_key>) and replays as a\n    bearer token.\ntoken_lifecycle:\n  caching: client-side, keyed on the API key\n  refresh_trigger: >-\n    A 401 Not Authorized on any resource request causes the client to request a\n    new access token and retry once before surfacing the error.\n  expiry_published: false\ncredentials:\n  issuance: private — issued by CarServ to integrating accounts; no public self-serve signup\n  rotation_policy_published:\
  \ false\nstatus: discontinued\nstatus_note: >-\n  The authentication host is no longer resolvable; carserv.com is a parked domain.\n  This profile documents the historical contract as shipped in the client library.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carserv/refs/heads/main/authentication/carserv-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Auto Repair
- Shop Management
- Vehicle Inspection
- Field Service
- SaaS
- JSON API
- Defunct
---
