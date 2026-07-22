---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Meritfirst Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meritfirst secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Meritfirst
provider_slug: meritfirst
scheme_count: 1
schemes:
- description: MeritFirst authenticates API/MCP access with a personal API key that begins with mf_, presented as an HTTP Bearer token in the Authorization header. Keys are generated in the account UI under Settings > API Keys.
  format: Bearer <api_key>
  header_name: Authorization
  in: header
  key_prefix: mf_
  name: MeritFirstApiKey
  provisioning: Settings > API Keys
  sources:
  - well-known/meritfirst-api-catalog.json
  - mcp/meritfirst-server-card.json
  type: apiKey
slug: meritfirst-authentication
source_filename: meritfirst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.meritfirst.us/.well-known/mcp/server-card.json\ndocs: null\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_scheme: bearer\n  oauth2_flows: []\nschemes:\n  - name: MeritFirstApiKey\n    type: apiKey\n    in: header\n    header_name: Authorization\n    format: 'Bearer <api_key>'\n    key_prefix: mf_\n    provisioning: Settings > API Keys\n    description: >-\n      MeritFirst authenticates API/MCP access with a personal API key that\n      begins with mf_, presented as an HTTP Bearer token in the Authorization\n      header. Keys are generated in the account UI under Settings > API Keys.\n    sources:\n      - well-known/meritfirst-api-catalog.json\n      - mcp/meritfirst-server-card.json\nnotes: >-\n  Derived from the MCP server card (the only public machine-readable auth\n  descriptor MeritFirst publishes); no OpenAPI is available to run\n  derive-authentication.py against. No OAuth authorization-server\
  \ or\n  openid-configuration is exposed (both /.well-known probes 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meritfirst/refs/heads/main/authentication/meritfirst-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Hiring
- Recruiting
- Assessments
- Talent
- Skills-Based Hiring
- MCP
---
