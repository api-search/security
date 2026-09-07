---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 30mhz-zensie-openapi.json
  format: json
  label: ZENSIE API
  slug: zensie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/openapi/30mhz-zensie-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 30Mhz Authentication
name_suffix: Authentication
oauth_flows: []
overview: 30MHz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 30MHz
provider_slug: 30mhz
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/30mhz-zensie-openapi.json
  type: apiKey
slug: 30mhz-authentication
source_filename: 30mhz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/30mhz-zensie-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/30mhz-zensie-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/authentication/30mhz-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Horticulture
- Agriculture
- AgTech
- Sensors
- Internet of Things
- Greenhouse
- Climate Monitoring
- Time Series Data
- Data Platform
- Netherlands
---
