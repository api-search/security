---
api_key_in:
- header
api_specs:
- filename: weld-connect-openapi.json
  format: json
  label: Weld Connect API
  slug: weld-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-connect-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weld secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weld
provider_slug: weld
scheme_count: 1
schemes:
- description: The API key from Settings -> API Keys
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/weld-connect-openapi.json
  type: apiKey
slug: weld-authentication
source_filename: weld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/weld-connect-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The API key from Settings -> API Keys\n  sources:\n  - openapi/weld-connect-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/authentication/weld-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- ETL
- ELT
- Reverse ETL
- Data Pipelines
- Data Integration
- Change Data Capture
- Transformations
- Analytics
- MCP
- AI Agents
---
