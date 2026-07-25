---
api_key_in: []
api_specs:
- filename: ditto-live-api-keys-api-openapi.yml
  format: yaml
  label: Ditto API Keys API
  slug: ditto-live-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-api-keys-api-openapi.yml
- filename: ditto-live-apps-api-openapi.yml
  format: yaml
  label: Ditto Apps API
  slug: ditto-live-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-apps-api-openapi.yml
- filename: ditto-live-bigpeerreplication-api-openapi.yml
  format: yaml
  label: Ditto BigPeerReplication API
  slug: ditto-live-bigpeerreplication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-bigpeerreplication-api-openapi.yml
- filename: ditto-live-data-bridge-api-openapi.yml
  format: yaml
  label: Ditto Data Bridge API
  slug: ditto-live-data-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-data-bridge-api-openapi.yml
- filename: ditto-live-store-api-openapi.yml
  format: yaml
  label: Ditto Store API
  slug: ditto-live-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-store-api-openapi.yml
- filename: ditto-live-sync-api-openapi.yml
  format: yaml
  label: Ditto Sync API
  slug: ditto-live-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ditto-live/refs/heads/main/openapi/ditto-live-sync-api-openapi.yml
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
