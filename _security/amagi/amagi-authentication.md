---
api_key_in:
- header
- query
api_specs:
- filename: amagi-mapsor-openapi.yml
  format: yaml
  label: Mapsor API
  slug: mapsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-mapsor-openapi.yml
- filename: amagi-callisto-openapi.yml
  format: yaml
  label: services-amagi-tv API
  slug: services-amagi-tv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-callisto-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amagi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amagi secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amagi
provider_slug: amagi
scheme_count: 3
schemes:
- in: header
  name: access-key
  parameter: access_key
  sources:
  - openapi/amagi-callisto-openapi.yml
  type: apiKey
- in: header
  name: secret-key
  parameter: secret_key
  sources:
  - openapi/amagi-callisto-openapi.yml
  type: apiKey
- in: query
  name: TokenAuth
  parameter: token
  sources:
  - openapi/amagi-mapsor-openapi.yml
  type: apiKey
slug: amagi-authentication
source_filename: amagi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/amagi-callisto-openapi.yml, openapi/amagi-mapsor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: access-key\n  type: apiKey\n  in: header\n  parameter: access_key\n  sources:\n  - openapi/amagi-callisto-openapi.yml\n- name: secret-key\n  type: apiKey\n  in: header\n  parameter: secret_key\n  sources:\n  - openapi/amagi-callisto-openapi.yml\n- name: TokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/amagi-mapsor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/authentication/amagi-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Media
- Broadcast
- Streaming
- Video
- CTV
- FAST
- Advertising
- Cloud
- Playout
---
