---
api_key_in:
- header
api_specs:
- filename: ubicquia-config-api-openapi-original.json
  format: json
  label: Ubicquia Config API
  slug: ubicquia-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-config-api-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ubicquia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubicquia secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ubicquia
provider_slug: ubicquia
scheme_count: 1
schemes:
- description: 'Use header x-api-key: ''key'' to send api key endpoints'
  in: header
  name: Api Key
  parameter: x-api-key
  sources:
  - openapi/ubicquia-config-api-openapi-original.json
  type: apiKey
slug: ubicquia-authentication
source_filename: ubicquia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nsource: openapi/ubicquia-config-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Api Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Use header x-api-key: ''key'' to send api key endpoints'\n  sources:\n  - openapi/ubicquia-config-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/authentication/ubicquia-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Smart Cities
- Internet of Things
- Energy
- Utilities
- Electric Grid
- Streetlights
- Public Safety
- Infrastructure
- Sensors
- Edge AI
- Transformer Monitoring
---
