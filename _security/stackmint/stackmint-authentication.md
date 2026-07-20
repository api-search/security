---
api_key_in:
- header
api_specs:
- filename: stackmint-openapi.yml
  format: yaml
  label: Stackmint Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackmint/refs/heads/main/openapi/stackmint-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stackmint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stackmint secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stackmint
provider_slug: stackmint
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: 'Authorization: Bearer [example key]'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stackmint-openapi.yml
  type: http
- description: Stackmint organization identifier.
  in: header
  name: OrgId
  parameter: X-Stackmint-Org-Id
  sources:
  - openapi/stackmint-openapi.yml
  type: apiKey
slug: stackmint-authentication
source_filename: stackmint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackmint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'Authorization: Bearer [example key]'\n  sources:\n  - openapi/stackmint-openapi.yml\n- name: OrgId\n  type: apiKey\n  in: header\n  parameter: X-Stackmint-Org-Id\n  description: Stackmint organization identifier.\n  sources:\n  - openapi/stackmint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackmint/refs/heads/main/authentication/stackmint-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Governance
- AI Agents
- Workflow Automation
- Enterprise AI
- MCP
- Semantic Layer
- Audit
- Compliance
---
