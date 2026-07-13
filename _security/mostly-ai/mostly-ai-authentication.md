---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mostly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MOSTLY AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MOSTLY AI
provider_slug: mostly-ai
scheme_count: 1
schemes:
- description: API key issued from the user profile in the MOSTLY AI web app.
  in: header
  name: apiKey
  parameter: X-MOSTLY-API-KEY
  sources:
  - openapi/mostly-ai-openapi.yml
  type: apiKey
slug: mostly-ai-authentication
source_filename: mostly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mostly-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-MOSTLY-API-KEY\n  description: API key issued from the user profile in the MOSTLY AI web app.\n  sources:\n  - openapi/mostly-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/authentication/mostly-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Synthetic Data
- Privacy
- Tabular
- Differential Privacy
- Python SDK
- REST
- Apache 2.0
---
