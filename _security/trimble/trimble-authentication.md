---
api_key_in:
- header
api_specs:
- filename: trimble-connect-openapi.yml
  format: yaml
  label: Trimble Connect API
  slug: trimble-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-connect-openapi.yml
- filename: trimble-maps-openapi.yml
  format: yaml
  label: Trimble Maps API
  slug: trimble-maps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-maps-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trimble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trimble secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trimble
provider_slug: trimble
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Trimble Identity OAuth2 Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/trimble-connect-openapi.yml
  type: http
- description: 'Format: ALK apiKey'
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/trimble-maps-openapi.yml
  type: apiKey
slug: trimble-authentication
source_filename: trimble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trimble-connect-openapi.yml, openapi/trimble-maps-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Trimble Identity OAuth2 Bearer token\n  sources:\n  - openapi/trimble-connect-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format: ALK apiKey'\n  sources:\n  - openapi/trimble-maps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/authentication/trimble-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Construction
- Transportation
- Geospatial
- GPS
- Mapping
- BIM
- Fleet Management
- Collaboration
- Agriculture
---
