---
api_key_in: []
api_specs:
- filename: anduril-openapi.yml
  format: yaml
  label: Anduril Lattice SDK
  slug: lattice-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Anduril Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Anduril Industries secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Anduril Industries
provider_slug: anduril
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token issued via /oauth/token or partner-issued bearer.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anduril-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/anduril-openapi.yml
  type: oauth2
slug: anduril-authentication
source_filename: anduril-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anduril-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token issued via /oauth/token or partner-issued bearer.\n  sources:\n  - openapi/anduril-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials flow for service-to-service access.\n  sources:\n  - openapi/anduril-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/authentication/anduril-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Defense
- Autonomy
- Lattice
- Command and Control
- C2
- Sensors
- Effectors
- Counter-UAS
- Unmanned Systems
- Mission Software
- Edge AI
- ITAR
---
