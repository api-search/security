---
api_key_in: []
api_specs:
- filename: gojiberry-ai-external-openapi-original.json
  format: json
  label: Gojiberry AI External API
  slug: gojiberry-ai-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-external-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gojiberry Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gojiberry AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter API Key
  name: API-Key
  scheme: bearer
  sources:
  - openapi/gojiberry-ai-external-openapi-original.json
  type: http
slug: gojiberry-ai-authentication
source_filename: gojiberry-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gojiberry-ai-external-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: API-Key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter API Key\n  sources:\n  - openapi/gojiberry-ai-external-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/authentication/gojiberry-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
---
