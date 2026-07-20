---
api_key_in:
- header
api_specs:
- filename: fixie-ultravox-openapi-original.yml
  format: yaml
  label: Ultravox Realtime API
  slug: ultravox-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-ultravox-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fixie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fixie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fixie
provider_slug: fixie
scheme_count: 1
schemes:
- description: API key
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/fixie-ultravox-openapi-original.yml
  type: apiKey
slug: fixie-authentication
source_filename: fixie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fixie-ultravox-openapi-original.yml\ndocs: https://docs.ultravox.ai/gettingstarted/quickstart/api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Single auth model — a 41-character API key (8 chars + '.' + 32 chars) sent\n    in the X-API-Key request header. No OAuth or OIDC; there is no scope surface.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key\n  sources:\n  - openapi/fixie-ultravox-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/authentication/fixie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Voice AI
- Conversational AI
- Real-time
- Speech
- Agents
- Telephony
- Machine Learning
- SIP
- Webhooks
---
