---
api_key_in:
- header
api_specs:
- filename: emerge-tools-openapi.json
  format: json
  label: Emerge API
  slug: emerge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Emerge Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emerge Tools secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emerge Tools
provider_slug: emerge-tools
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Token
  sources:
  - openapi/emerge-tools-openapi.json
  type: apiKey
slug: emerge-tools-authentication
source_filename: emerge-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/emerge-tools-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Token\n  sources:\n  - openapi/emerge-tools-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/authentication/emerge-tools-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B
- Mobile
- Developer Tools
- App Performance
- Testing
- iOS
- Android
- DevOps
---
