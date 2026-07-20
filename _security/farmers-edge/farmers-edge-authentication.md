---
api_key_in:
- query
api_specs:
- filename: farmers-edge-farmcommand-openapi-original.json
  format: json
  label: FarmCommand API
  slug: farmcommand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/openapi/farmers-edge-farmcommand-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Farmers Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farmers Edge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Farmers Edge
provider_slug: farmers-edge
scheme_count: 1
schemes:
- in: query
  name: FarmCommand Token
  parameter: token
  sources:
  - openapi/farmers-edge-farmcommand-openapi-original.json
  type: apiKey
slug: farmers-edge-authentication
source_filename: farmers-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/farmers-edge-farmcommand-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: FarmCommand Token\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/farmers-edge-farmcommand-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-edge/refs/heads/main/authentication/farmers-edge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Agriculture
- Precision Agriculture
- AgTech
- Farm Management
- Digital Agriculture
- IoT
- Weather
- Carbon
- API
---
