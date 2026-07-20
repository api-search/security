---
api_key_in:
- header
api_specs:
- filename: airweave-openapi.json
  format: json
  label: Airweave API
  slug: airweave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airweave/refs/heads/main/openapi/airweave-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Airweave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airweave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airweave
provider_slug: airweave
scheme_count: 1
schemes:
- in: header
  name: default
  parameter: x-api-key
  sources:
  - openapi/airweave-openapi.json
  type: apiKey
slug: airweave-authentication
source_filename: airweave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/airweave-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: default\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/airweave-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airweave/refs/heads/main/authentication/airweave-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Search
- RAG
- Retrieval
- Agents
- MCP
- Vector Search
- Data Integration
- Context
---
