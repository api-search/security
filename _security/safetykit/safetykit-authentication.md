---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Safetykit Authentication
name_suffix: Authentication
oauth_flows: []
overview: SafetyKit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SafetyKit
provider_slug: safetykit
scheme_count: 1
schemes:
- description: All SafetyKit API calls authenticate with a bearer token in the Authorization header. API keys are prefixed with `sk_` and are created on the Team API Keys page in the SafetyKit dashboard. Keys are server-side secrets and must never be exposed to client-side code (browsers, mobile apps); browser/mobile SDK access is brokered through short-lived session tokens minted server-side via POST /v1/sessions.
  header_example: 'Authorization: Bearer sk_...'
  key_prefix: sk_
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.safetykit.com/authentication
  type: http
slug: safetykit-authentication
source_filename: safetykit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.safetykit.com/authentication\ndocs: https://docs.safetykit.com/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All SafetyKit API calls authenticate with a bearer token in the Authorization\n    header. API keys are prefixed with `sk_` and are created on the Team API Keys\n    page in the SafetyKit dashboard. Keys are server-side secrets and must never be\n    exposed to client-side code (browsers, mobile apps); browser/mobile SDK access\n    is brokered through short-lived session tokens minted server-side via POST /v1/sessions.\n  header_example: 'Authorization: Bearer sk_...'\n  key_prefix: sk_\n  sources:\n  - https://docs.safetykit.com/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safetykit/refs/heads/main/authentication/safetykit-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Trust and Safety
- Fraud Detection
- Content Moderation
- Risk
- AI Agents
- Compliance
---
