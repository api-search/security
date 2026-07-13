---
api_key_in:
- header
api_specs:
- filename: flasharray-rest-api-openapi.yml
  format: yaml
  label: FlashArray REST API
  slug: flasharray-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/flasharray-rest-api-openapi.yml
- filename: flashblade-rest-api-openapi.yml
  format: yaml
  label: FlashBlade REST API
  slug: flashblade-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/flashblade-rest-api-openapi.yml
- filename: pure1-cloud-api-openapi.yml
  format: yaml
  label: Pure1 Public REST API
  slug: pure1-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/openapi/pure1-cloud-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pure Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pure Storage secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pure Storage
provider_slug: pure-storage
scheme_count: 3
schemes:
- in: header
  name: AuthorizationHeader
  parameter: x-auth-token
  sources:
  - openapi/flashblade-rest-api-openapi.yml
  type: apiKey
- in: header
  name: ApiToken
  parameter: api-token
  sources:
  - openapi/flashblade-rest-api-openapi.yml
  type: apiKey
- in: header
  name: AuthorizationHeader
  parameter: Authorization
  sources:
  - openapi/pure1-cloud-api-openapi.yml
  type: apiKey
slug: pure-storage-authentication
source_filename: pure-storage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flashblade-rest-api-openapi.yml, openapi/pure1-cloud-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthorizationHeader\n  type: apiKey\n  in: header\n  parameter: x-auth-token\n  sources:\n  - openapi/flashblade-rest-api-openapi.yml\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: api-token\n  sources:\n  - openapi/flashblade-rest-api-openapi.yml\n- name: AuthorizationHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/pure1-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pure-storage/refs/heads/main/authentication/pure-storage-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Storage
- Data Storage
- Flash Storage
- Enterprise Storage
- Cloud Storage
- Object Storage
- File Storage
- Block Storage
- Kubernetes Storage
- Infrastructure
---
