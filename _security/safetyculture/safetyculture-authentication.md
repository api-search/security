---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Safetyculture Authentication
name_suffix: Authentication
oauth_flows: []
overview: SafetyCulture secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SafetyCulture
provider_slug: safetyculture
scheme_count: 1
schemes:
- format: 'Authorization: Bearer {api_token}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.safetyculture.com/reference/authentication
  type: http
slug: safetyculture-authentication
source_filename: safetyculture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.safetyculture.com/reference/authentication\ndocs: https://developer.safetyculture.com/reference/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    No OAuth 2.0 authorization flow. Access is a bearer API token whose effective\n    permissions mirror the token owner's role, permission sets, and access rules.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {api_token}'\n  sources: [https://developer.safetyculture.com/reference/authentication]\ntoken_kinds:\n- kind: service_user_token\n  description: >-\n    Shared integration / long-running automation token. Up to 20 active tokens per\n    organization. Configurable inactivity expiry (31, 45, 60, or 180 days). Scoped by\n    selected permission sets.\n  generate_at: Organization > Integrations > API tokens\n\
  - kind: user_token\n  description: >-\n    Personal token whose access mirrors a specific user. Up to 10 active tokens per\n    user. Expires after 30 days of inactivity.\n  generate_at: My Profile > Settings > API tokens\nauthorization_model: >-\n  The API only returns or changes data the token owner can access, evaluated through\n  permissions (which actions are allowed) and access rules (which items are visible).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safetyculture/refs/heads/main/authentication/safetyculture-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Business Applications
- Safety
- Inspections
- Workplace Operations
- EHS
- Compliance
- Training
- Field Service
- Webhooks
---
