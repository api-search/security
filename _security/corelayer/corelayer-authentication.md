---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Corelayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corelayer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Corelayer
provider_slug: corelayer
scheme_count: 1
schemes:
- description: Corelayer v1 REST API authenticates with an API key sent as a bearer token in the Authorization header. Keys are created from the dashboard (Settings > API Keys) or via the API (POST /api/v1/api-keys), shown once, and can carry an optional expiration. Access is governed by role-based access control (RBAC) with per-key rate limiting and configurable tiers.
  format: Bearer <api-key>
  header: Authorization
  in: header
  key_prefixes:
  - cl_live_
  - cl_key_
  - clr_
  name: apiKey
  sources:
  - docs
  type: apiKey
slug: corelayer-authentication
source_filename: corelayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.corelayer.com/cli/overview + https://docs.corelayer.com/anomalies/sdk-metrics + changelog v1.3.0\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  rbac: true\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  format: Bearer <api-key>\n  key_prefixes: [cl_live_, cl_key_, clr_]\n  description: >-\n    Corelayer v1 REST API authenticates with an API key sent as a bearer token\n    in the Authorization header. Keys are created from the dashboard\n    (Settings > API Keys) or via the API (POST /api/v1/api-keys), shown once,\n    and can carry an optional expiration. Access is governed by role-based\n    access control (RBAC) with per-key rate limiting and configurable tiers.\n  sources: [docs]\nbrowser_login:\n  description: >-\n    The CLI supports an interactive browser OAuth-style authorization flow\n    (corelayer login) that authorizes CLI access for the\
  \ current organization\n    and stores the resulting API key + server URL in ~/.corelayer/config.json.\n  auth_server: https://app.corelayer.com\ncredential_resolution_order:\n- CORELAYER_API_KEY environment variable\n- token stored in ~/.corelayer/config.json (from corelayer login)\nnotes: >-\n  Legacy internal HMAC authentication was removed in v1.3.0 (March 2026) in\n  favor of API key auth. No OAuth2/OIDC scopes surface is published; scopes/ is\n  intentionally omitted (key-auth + RBAC, not OAuth scopes).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelayer/refs/heads/main/authentication/corelayer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- SRE
- Incident Response
- Observability
- Production Support
- Root Cause Analysis
- Anomaly Detection
- DevOps
- Agent Native
- MCP
- Fintech
---
