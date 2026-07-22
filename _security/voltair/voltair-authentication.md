---
api_key_in:
- header
api_specs:
- filename: voltair-api-openapi-original.yml
  format: yaml
  label: Voltair API
  slug: voltair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-api-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voltair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltair secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voltair
provider_slug: voltair
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Cognito JWT access token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/voltair-api-openapi-original.yml
  type: http
- description: Organization-scoped API key
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/voltair-api-openapi-original.yml
  type: apiKey
slug: voltair-authentication
source_filename: voltair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/voltair-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Cognito JWT access token\n  sources:\n  - openapi/voltair-api-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organization-scoped API key\n  sources:\n  - openapi/voltair-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/authentication/voltair-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Drones
- Earth Observation
- Infrastructure Inspection
- Utilities
- Energy
- Robotics
- LiDAR
- Aerial Imagery
---
