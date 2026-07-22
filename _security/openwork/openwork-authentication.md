---
api_key_in:
- header
api_specs:
- filename: openwork-den-openapi.json
  format: json
  label: OpenWork Den API
  slug: den-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/openapi/openwork-den-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openwork secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Openwork
provider_slug: openwork
scheme_count: 2
schemes:
- bearerFormat: session-token
  description: 'Session token passed as `Authorization: Bearer <session-token>` for user-authenticated Den routes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openwork-den-openapi.json
  type: http
- description: Organization API key passed as the `x-api-key` header for API-key-authenticated Den routes.
  in: header
  name: denApiKey
  parameter: x-api-key
  sources:
  - openapi/openwork-den-openapi.json
  type: apiKey
slug: openwork-authentication
source_filename: openwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/openwork-den-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: session-token\n  description: 'Session token passed as `Authorization: Bearer <session-token>` for user-authenticated\n    Den routes.'\n  sources:\n  - openapi/openwork-den-openapi.json\n- name: denApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Organization API key passed as the `x-api-key` header for API-key-authenticated\n    Den routes.\n  sources:\n  - openapi/openwork-den-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/authentication/openwork-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI Agents
- Open Source
- Desktop
- Agent Runtime
- MCP
- Control Plane
- SSO
- SCIM
- Developer Tools
---
