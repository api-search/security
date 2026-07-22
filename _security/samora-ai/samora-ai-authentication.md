---
api_key_in:
- header
api_specs:
- filename: samora-ai-openapi.yml
  format: yaml
  label: Samora AI API
  slug: samora-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samora-ai/refs/heads/main/openapi/samora-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Samora Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Samora AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Samora AI
provider_slug: samora-ai
scheme_count: 1
schemes:
- description: Organization API key. Server-to-server only; never expose in browser or mobile clients.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/samora-ai-openapi.yml
  type: apiKey
slug: samora-ai-authentication
source_filename: samora-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/samora-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organization API key. Server-to-server only; never expose in browser or mobile\n    clients.\n  sources:\n  - openapi/samora-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samora-ai/refs/heads/main/authentication/samora-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Voice Agents
- Conversational AI
- Voice AI
- Telephony
- Customer Communications
- Contact Center
- Campaigns
- Webhooks
---
