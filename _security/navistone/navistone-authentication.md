---
api_key_in:
- header
api_specs:
- filename: navistone-openapi-original.json
  format: json
  label: NaviStone Platform API
  slug: navistone-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Navistone Authentication
name_suffix: Authentication
oauth_flows: []
overview: NaviStone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NaviStone
provider_slug: navistone
scheme_count: 1
schemes:
- description: API Key for authentication
  in: header
  name: api-key
  parameter: X-API-Key
  sources:
  - openapi/navistone-openapi-original.json
  type: apiKey
slug: navistone-authentication
source_filename: navistone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/navistone-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key for authentication\n  sources:\n  - openapi/navistone-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/authentication/navistone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketing
- Direct Mail
- Advertising
- Customer Acquisition
- Audience Targeting
- MarTech
- AdTech
- Postcards
- Retargeting
---
