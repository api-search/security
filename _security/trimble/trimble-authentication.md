---
api_key_in:
- header
api_specs:
- filename: trimble-bcf-topics-api-openapi.yml
  format: yaml
  label: Trimble BCF Topics API
  slug: trimble-bcf-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-bcf-topics-api-openapi.yml
- filename: trimble-files-api-openapi.yml
  format: yaml
  label: Trimble Files API
  slug: trimble-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-files-api-openapi.yml
- filename: trimble-geocoding-api-openapi.yml
  format: yaml
  label: Trimble Geocoding API
  slug: trimble-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-geocoding-api-openapi.yml
- filename: trimble-projects-api-openapi.yml
  format: yaml
  label: Trimble Projects API
  slug: trimble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-projects-api-openapi.yml
- filename: trimble-routing-api-openapi.yml
  format: yaml
  label: Trimble Routing API
  slug: trimble-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-routing-api-openapi.yml
- filename: trimble-users-api-openapi.yml
  format: yaml
  label: Trimble Users API
  slug: trimble-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble/refs/heads/main/openapi/trimble-users-api-openapi.yml
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
