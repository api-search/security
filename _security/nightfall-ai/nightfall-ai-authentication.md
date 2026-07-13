---
api_key_in:
- header
api_specs:
- filename: nightfall-ai-openapi.yml
  format: yaml
  label: Nightfall AI
  slug: nightfall-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nightfall-ai/refs/heads/main/openapi/nightfall-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nightfall Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nightfall AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nightfall AI
provider_slug: nightfall-ai
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/nightfall-ai-openapi.yml
  type: apiKey
slug: nightfall-ai-authentication
source_filename: nightfall-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nightfall-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/nightfall-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nightfall-ai/refs/heads/main/authentication/nightfall-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Privacy
- Sensitive Data
---
