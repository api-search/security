---
api_key_in:
- header
api_specs:
- filename: eventxtra-public-api-openapi.json
  format: json
  label: EventX Public API
  slug: eventx-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/openapi/eventxtra-public-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eventxtra Authentication
name_suffix: Authentication
oauth_flows: []
overview: EventX secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EventX
provider_slug: eventxtra
scheme_count: 1
schemes:
- description: Bearer Authorization with jwt token
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/eventxtra-public-api-openapi.json
  type: apiKey
slug: eventxtra-authentication
source_filename: eventxtra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/eventxtra-public-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer Authorization with jwt token\n  sources:\n  - openapi/eventxtra-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventxtra/refs/heads/main/authentication/eventxtra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Event Management
- Event Registration
- Ticketing
- Check-in
- Event Marketing
- Virtual Events
- Webhook
- OpenAPI
- MCP
- Artificial Intelligence
- Hong Kong
- APAC
---
