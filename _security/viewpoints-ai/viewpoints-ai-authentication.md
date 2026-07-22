---
api_key_in:
- header
api_specs:
- filename: viewpoints-ai-study-openapi.json
  format: json
  label: Viewpoints Study API
  slug: viewpoints-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/openapi/viewpoints-ai-study-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Viewpoints Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Viewpoints AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Viewpoints AI
provider_slug: viewpoints-ai
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/viewpoints-ai-study-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/viewpoints-ai-study-openapi.json
  type: http
slug: viewpoints-ai-authentication
source_filename: viewpoints-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/viewpoints-ai-study-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/viewpoints-ai-study-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/viewpoints-ai-study-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/authentication/viewpoints-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Market Research
- Synthetic Personas
- Consumer Insights
- Litigation
- Jury Simulation
- Research
---
