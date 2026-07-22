---
api_key_in:
- header
api_specs:
- filename: notyfi-openapi-original.json
  format: json
  label: Notyfi API
  slug: notyfi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notyfi/refs/heads/main/openapi/notyfi-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notyfi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notyfi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Notyfi
provider_slug: notyfi
scheme_count: 2
schemes:
- description: 'Notyfi API key: `Authorization: Bearer notyfi_mk_...`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/notyfi-openapi-original.json
  type: http
- description: Notyfi API key as X-Api-Key.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/notyfi-openapi-original.json
  type: apiKey
slug: notyfi-authentication
source_filename: notyfi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/notyfi-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Notyfi API key: `Authorization: Bearer notyfi_mk_...`'\n  sources:\n  - openapi/notyfi-openapi-original.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Notyfi API key as X-Api-Key.\n  sources:\n  - openapi/notyfi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notyfi/refs/heads/main/authentication/notyfi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Notifications
- Monitoring
- Webhooks
- Real Time
- Agents
- MCP
- Alerts
---
