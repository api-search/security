---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bolna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bolna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bolna
provider_slug: bolna
scheme_count: 1
schemes:
- description: 'All Bolna API endpoints require authentication using an API key, sent in the Authorization header using the Bearer scheme: `Authorization: Bearer <BOLNA_API_KEY>`. API keys are generated in the Bolna dashboard (platform.bolna.ai) and are hashed at rest — Bolna cannot recover a plaintext key. A 401 is returned for a missing or invalid key; 403 for a valid key with insufficient permissions.'
  in: header
  key_name: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - https://www.bolna.ai/docs/api-reference/introduction
  type: http
slug: bolna-authentication
source_filename: bolna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.bolna.ai/docs/api-reference/introduction\ndocs: https://www.bolna.ai/docs/api-reference/introduction\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All Bolna API endpoints require authentication using an API key, sent in the\n    Authorization header using the Bearer scheme:\n    `Authorization: Bearer <BOLNA_API_KEY>`. API keys are generated in the Bolna\n    dashboard (platform.bolna.ai) and are hashed at rest — Bolna cannot recover a\n    plaintext key. A 401 is returned for a missing or invalid key; 403 for a\n    valid key with insufficient permissions.\n  in: header\n  key_name: Authorization\n  sources: [https://www.bolna.ai/docs/api-reference/introduction]\nnotes: >-\n  Key-auth provider (single Bearer API key). No OAuth2/OIDC scope surface, so no\n  scopes/ artifact. The\
  \ hosted MCP server (mcp/bolna-mcp.yml) accepts the same\n  Bearer API key (and optionally OAuth).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolna/refs/heads/main/authentication/bolna-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Voice AI
- Conversational AI
- Voice Agents
- Telephony
- Speech
- Call Automation
- Contact Center
- MCP
---
