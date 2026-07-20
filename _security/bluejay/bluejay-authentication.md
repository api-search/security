---
api_key_in:
- header
api_specs:
- filename: bluejay-openapi-original.json
  format: json
  label: Bluejay API
  slug: bluejay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay/refs/heads/main/openapi/bluejay-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bluejay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluejay secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bluejay
provider_slug: bluejay
scheme_count: 1
schemes:
- description: API key required to authenticate requests.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/bluejay-openapi-original.json
  type: apiKey
slug: bluejay-authentication
source_filename: bluejay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bluejay-openapi-original.json\ndocs: https://docs.getbluejay.ai/api-reference/introduction\nnotes: >-\n  Single API-key scheme. Generate a key from the app Settings > API Keys page\n  (https://app.getbluejay.ai/settings/api-keys) and pass it in the X-API-Key\n  request header. Applied globally as the root security requirement. No OAuth2\n  or OpenID Connect surface is published, so there is no scope model.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key required to authenticate requests.\n  sources:\n  - openapi/bluejay-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluejay/refs/heads/main/authentication/bluejay-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- AI Agents
- Voice AI
- Conversational AI
- Agent Testing
- Quality Assurance
- Observability
- Simulation
- Evaluation
- Monitoring
---
