---
api_key_in:
- header
api_specs:
- filename: deeptrace-api-openapi.yml
  format: yaml
  label: Deeptrace REST API
  slug: deeptrace-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeptrace/refs/heads/main/openapi/deeptrace-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Deeptrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deeptrace secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Deeptrace
provider_slug: deeptrace
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  prefix: dt_
  sources:
  - https://docs.deeptrace.com/trigger-investigation
  type: apiKey
- description: 'Authorization: Bearer <your_api_key> — the same Deeptrace API key.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.deeptrace.com/send-chat
  - https://docs.deeptrace.com/get-chat
  type: http
slug: deeptrace-authentication
source_filename: deeptrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.deeptrace.com/api.md\ndocs: https://docs.deeptrace.com/trigger-investigation\nsummary:\n  types: [apiKey, http-bearer]\n  api_key_in: [header]\n  api_key_header: X-API-Key\n  api_key_prefix: dt_\n  oauth2_flows: []\n  notes: >-\n    A single Deeptrace API key authenticates every REST endpoint. It may be sent\n    either as the X-API-Key header or as an Authorization: Bearer <key> token — the\n    two are interchangeable. Keys are created and revoked in the dashboard at\n    Settings > API Keys (https://app.deeptrace.com/api-keys). Dashboard/web app\n    sign-in is handled separately by Clerk (clerk.deeptrace.com); the API key is the\n    programmatic credential.\nschemes:\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    prefix: dt_\n    sources: [https://docs.deeptrace.com/trigger-investigation]\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: 'Authorization:\
  \ Bearer <your_api_key> — the same Deeptrace API key.'\n    sources: [https://docs.deeptrace.com/send-chat, https://docs.deeptrace.com/get-chat]\nkey_management:\n  create: https://app.deeptrace.com/api-keys\n  settings: https://app.deeptrace.com/settings\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deeptrace/refs/heads/main/authentication/deeptrace-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Company
- AIOps
- Site Reliability Engineering
- Observability
- Incident Management
- Root Cause Analysis
- Monitoring
- DevOps
- AI Agent
---
