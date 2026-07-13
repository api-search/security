---
api_key_in: []
api_specs:
- filename: microsoft-sentinel-openapi.yml
  format: yaml
  label: Microsoft Sentinel REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-sentinel/refs/heads/main/openapi/microsoft-sentinel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Sentinel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Sentinel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Sentinel
provider_slug: microsoft-sentinel
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/microsoft-sentinel-openapi.yml
  type: http
slug: microsoft-sentinel-authentication
source_filename: microsoft-sentinel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-sentinel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/microsoft-sentinel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-sentinel/refs/heads/main/authentication/microsoft-sentinel-authentication.yml
summary_line: http · 1 scheme
tags:
- Microsoft
- Security
- SIEM
- SOAR
- Threat Detection
---
