---
api_key_in: []
api_specs:
- filename: frontline-openapi-original.yml
  format: yaml
  label: Frontline Public API
  slug: frontline-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontline/refs/heads/main/openapi/frontline-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Frontline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frontline secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Frontline
provider_slug: frontline
scheme_count: 2
schemes:
- bearerFormat: Account API Key
  description: Account-level API key (GENERAL). Authenticates on behalf of the entire account with no user identity. Use for read-only integrations, dashboards, and machine-to-machine sync. Created in the app under Account settings > Developer. No fixed per-account cap.
  key_type: GENERAL
  name: accountApiKey
  scheme: bearer
  sources:
  - openapi/frontline-openapi-original.yml
  type: http
- bearerFormat: User API Key
  description: User-level API key (USER). Authenticates on behalf of a specific user. Required for write operations and user-owned resources; also accepted on all account-level endpoints. Created in the app under My settings > Bring your own Agent. Up to 5 personal keys per user.
  key_type: USER
  name: userApiKey
  scheme: bearer
  sources:
  - openapi/frontline-openapi-original.yml
  type: http
slug: frontline-authentication
source_filename: frontline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/frontline-openapi-original.yml\ndocs: https://docs.getfrontline.ai/docs/authentication.md\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_location: Authorization header (Bearer)\n  oauth2_flows: []\nschemes:\n- name: accountApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Account API Key\n  key_type: GENERAL\n  description: >-\n    Account-level API key (GENERAL). Authenticates on behalf of the entire account with no user\n    identity. Use for read-only integrations, dashboards, and machine-to-machine sync. Created in\n    the app under Account settings > Developer. No fixed per-account cap.\n  sources:\n  - openapi/frontline-openapi-original.yml\n- name: userApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: User API Key\n  key_type: USER\n  description: >-\n    User-level API key (USER). Authenticates on behalf of a specific user. Required for write\n    operations and user-owned\
  \ resources; also accepted on all account-level endpoints. Created in\n    the app under My settings > Bring your own Agent. Up to 5 personal keys per user.\n  sources:\n  - openapi/frontline-openapi-original.yml\ntransport: HTTPS/TLS only\nkey_handling:\n  display: One-time display on creation; only a SHA-256 hash is stored server-side.\n  rotation: No in-place rotation — create new, swap, delete old.\n  revocation: Deleting a key invalidates it on the next request, no grace period.\nverify:\n  operation: getMe\n  request: 'GET /public/v1/me with Authorization: Bearer <key>'\n  note: data.user is null for GENERAL keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontline/refs/heads/main/authentication/frontline-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- CRM
- AI Agents
- Sales Automation
- Customer Support
- Workflows
- Conversational AI
---
