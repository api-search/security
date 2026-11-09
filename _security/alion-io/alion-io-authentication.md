---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: alion-io-mcp-api-openapi.yml
  format: yaml
  label: Alion MCP API
  slug: alion-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alion-io/openapi/alion-io-mcp-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Alion Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alion secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alion
provider_slug: alion-io
scheme_count: 2
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/alion-io-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/alion-io-openapi.json
  type: apiKey
slug: alion-io-authentication
source_filename: alion-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/alion-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/alion-io-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/alion-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alion-io/authentication/alion-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Market Intelligence
- Companies
- Job
- Data-Graph
---
