---
api_key_in:
- header
api_specs:
- filename: sail-research-openapi-original.json
  format: json
  label: Sail API
  slug: sail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail-research/refs/heads/main/openapi/sail-research-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sail Research Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sail Research secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sail Research
provider_slug: sail-research
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sail-research-openapi-original.json
  type: http
slug: sail-research-authentication
source_filename: sail-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sail-research-openapi-original.json\ndocs: https://docs.sailresearch.com/quickstart\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nnotes: >-\n  Auth is a bearer API key. Send 'Authorization: Bearer $SAIL_API_KEY'. Keys are\n  created/managed at app.sailresearch.com. Sail is OpenAI- and Anthropic-SDK compatible,\n  so the same key drops into those clients by changing the base URL to\n  https://api.sailresearch.com/v1. No OAuth2 / scopes surface.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/sail-research-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sail-research/refs/heads/main/authentication/sail-research-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Inference
- Agents
- Machine Learning
- Developer Tools
---
