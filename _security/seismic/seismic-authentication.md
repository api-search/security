---
api_key_in: []
api_specs:
- filename: seismic-content-openapi.yml
  format: yaml
  label: Seismic Content API
  slug: seismic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-openapi.yml
- filename: seismic-livedocs-openapi.yml
  format: yaml
  label: Seismic LiveDocs API
  slug: seismic-livedocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-livedocs-openapi.yml
- filename: seismic-analytics-openapi.yml
  format: yaml
  label: Seismic Analytics API
  slug: seismic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-analytics-openapi.yml
- filename: seismic-user-management-openapi.yml
  format: yaml
  label: Seismic User Management API
  slug: seismic-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-user-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Seismic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seismic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seismic
provider_slug: seismic
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer Token. Obtain tokens through the Seismic authentication flow. See https://developer.seismic.com/seismicsoftware/docs/authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/seismic-analytics-openapi.yml
  - openapi/seismic-content-openapi.yml
  - openapi/seismic-livedocs-openapi.yml
  - openapi/seismic-user-management-openapi.yml
  type: http
slug: seismic-authentication
source_filename: seismic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seismic-analytics-openapi.yml, openapi/seismic-content-openapi.yml, openapi/seismic-livedocs-openapi.yml,\n  openapi/seismic-user-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer Token. Obtain tokens through the Seismic authentication flow.\n    See https://developer.seismic.com/seismicsoftware/docs/authentication\n  sources:\n  - openapi/seismic-analytics-openapi.yml\n  - openapi/seismic-content-openapi.yml\n  - openapi/seismic-livedocs-openapi.yml\n  - openapi/seismic-user-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/authentication/seismic-authentication.yml
summary_line: http · 1 scheme
tags: []
---
