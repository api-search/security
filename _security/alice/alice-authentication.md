---
api_key_in:
- header
api_specs:
- filename: alice-openapi-original.json
  format: json
  label: Alice API
  slug: alice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Alice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alice secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alice
provider_slug: alice
scheme_count: 1
schemes:
- description: ''
  in: header
  name: API Key
  parameter: af-api-key
  sources:
  - openapi/alice-openapi-original.json
  type: apiKey
slug: alice-authentication
source_filename: alice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/alice-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: af-api-key\n  description: ''\n  sources:\n  - openapi/alice-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/authentication/alice-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- AI Security
- AI Safety
- Content Moderation
- Trust and Safety
- LLM Guardrails
- Red Teaming
- GenAI
---
