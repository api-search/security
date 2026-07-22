---
api_key_in:
- header
api_specs:
- filename: yutori-openapi-original.json
  format: json
  label: Yutori API
  slug: yutori-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yutori/refs/heads/main/openapi/yutori-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yutori Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yutori secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yutori
provider_slug: yutori
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/yutori-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  description: 'Use Authorization: Bearer <api_key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/yutori-openapi-original.json
  type: http
slug: yutori-authentication
source_filename: yutori-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/yutori-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/yutori-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Use Authorization: Bearer <api_key>'\n  sources:\n  - openapi/yutori-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yutori/refs/heads/main/authentication/yutori-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Agents
- Web Automation
- Browser Automation
- Web Monitoring
- Research
- MCP
- LLM
---
