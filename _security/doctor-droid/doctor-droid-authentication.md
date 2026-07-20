---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Doctor Droid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doctor Droid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doctor Droid
provider_slug: doctor-droid
scheme_count: 1
schemes:
- description: DrDroid platform and MCP access is authenticated with a Bearer API key passed in the Authorization header. Keys are generated in the DrDroid dashboard under Settings > Proxy Tokens, API Keys & MCP.
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.drdroid.io/getting-started/drdroid-mcp-server
  type: http
slug: doctor-droid-authentication
source_filename: doctor-droid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.drdroid.io/getting-started/drdroid-mcp-server\ndocs: https://docs.drdroid.io/getting-started/drdroid-mcp-server\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_generation: Dashboard > Settings > Proxy Tokens, API Keys & MCP\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    DrDroid platform and MCP access is authenticated with a Bearer API key passed in the Authorization\n    header. Keys are generated in the DrDroid dashboard under Settings > Proxy Tokens, API Keys & MCP.\n  in: header\n  header: Authorization\n  sources: [https://docs.drdroid.io/getting-started/drdroid-mcp-server]\nnotes: >-\n  The DrDroid trust center at security.drdroid.io separately exposes an OAuth 2.0 authorization-server\n  (SafeBase-hosted, PKCE S256, authorization_code + refresh_token) for its own MCP endpoint — see\n  well-known/doctor-droid-oauth-authorization-server.json.\
  \ That is distinct from DrDroid platform auth,\n  which is the Bearer API key documented above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctor-droid/refs/heads/main/authentication/doctor-droid-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- AIOps
- SRE
- Incident Response
- On-Call
- Observability
- DevOps
- Monitoring
- MCP
---
