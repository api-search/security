---
api_key_in:
- header
api_specs:
- filename: relay-app-openapi.yml
  format: yaml
  label: Relay App Automation API
  slug: relay-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/openapi/relay-app-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Relay App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Relay App secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Relay App
provider_slug: relay-app
scheme_count: 1
schemes:
- description: API key for authenticating requests to the Relay App API.
  in: header
  name: ApiKeyAuth
  parameter: X-Relay-API-Key
  sources:
  - openapi/relay-app-openapi.yml
  type: apiKey
slug: relay-app-authentication
source_filename: relay-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/relay-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Relay-API-Key\n  description: API key for authenticating requests to the Relay App API.\n  sources:\n  - openapi/relay-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/authentication/relay-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Workflow
- Integration
- No-Code
- AI
- Webhooks
---
