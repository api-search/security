---
api_key_in: []
api_specs:
- filename: sumble-openapi-original.json
  format: json
  label: Sumble API
  slug: sumble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sumble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sumble secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sumble
provider_slug: sumble
scheme_count: 1
schemes:
- name: api_token
  scheme: bearer
  sources:
  - openapi/sumble-openapi-original.json
  type: http
slug: sumble-authentication
source_filename: sumble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sumble-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sumble-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/authentication/sumble-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
---
