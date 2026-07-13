---
api_key_in:
- header
api_specs:
- filename: api-spec.json
  format: json
  label: Eraser API
  slug: eraser-api
  spec_type: OpenAPI
  url: https://app.eraser.io/.well-known/api-spec.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Eraser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eraser secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eraser
provider_slug: eraser
scheme_count: 2
schemes:
- description: Team-specific API bearer token from Eraser settings
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eraser-eraser-api-openapi.yml
  type: http
- description: Audit-specific API key for accessing audit log endpoints
  in: header
  name: auditApiKey
  parameter: Authorization
  sources:
  - openapi/eraser-eraser-api-openapi.yml
  type: apiKey
slug: eraser-authentication
source_filename: eraser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eraser-eraser-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Team-specific API bearer token from Eraser settings\n  sources:\n  - openapi/eraser-eraser-api-openapi.yml\n- name: auditApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Audit-specific API key for accessing audit log endpoints\n  sources:\n  - openapi/eraser-eraser-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eraser/refs/heads/main/authentication/eraser-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Diagrams
- Documentation
- AI
- Technical Documentation
- Diagramming
- Architecture
- Developer Tools
---
