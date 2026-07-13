---
api_key_in:
- header
api_specs:
- filename: wallarm-openapi.yml
  format: yaml
  label: Wallarm API
  slug: wallarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wallarm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wallarm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wallarm
provider_slug: wallarm
scheme_count: 1
schemes:
- description: API token obtained from Wallarm Console under Settings → API Tokens.
  in: header
  name: ApiTokenAuth
  parameter: X-WallarmApi-Token
  sources:
  - openapi/wallarm-openapi.yml
  type: apiKey
slug: wallarm-authentication
source_filename: wallarm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wallarm-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-WallarmApi-Token\n  description: API token obtained from Wallarm Console under Settings → API Tokens.\n  sources:\n  - openapi/wallarm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/authentication/wallarm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Security
- Security Testing
- WAF
- Cybersecurity
---
