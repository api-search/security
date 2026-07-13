---
api_key_in: []
api_specs:
- filename: ditto-live-cloud-http-api-openapi.yml
  format: yaml
  label: Ditto Cloud HTTP API
  slug: cloud-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-cloud-http-api-openapi.yml
- filename: ditto-live-operator-api-openapi.yml
  format: yaml
  label: Ditto Edge Server HTTP API
  slug: edge-server-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-operator-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ditto Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ditto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ditto
provider_slug: ditto-live
scheme_count: 1
schemes:
- bearerFormat: API Key or JWT
  description: Authentication using either an API key or JWT token in the Authorization header
  name: api_key_or_jwt_token
  scheme: bearer
  sources:
  - openapi/ditto-live-cloud-http-api-openapi.yml
  type: http
slug: ditto-live-authentication
source_filename: ditto-live-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ditto-live-cloud-http-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_key_or_jwt_token\n  type: http\n  scheme: bearer\n  bearerFormat: API Key or JWT\n  description: Authentication using either an API key or JWT token in the Authorization header\n  sources:\n  - openapi/ditto-live-cloud-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/authentication/ditto-live-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Database
- Synchronization
- Peer-to-Peer
- Edge Computing
- Offline-First
- Mobile
---
