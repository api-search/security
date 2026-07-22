---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Uncodie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncodie (now Makinari) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uncodie (now Makinari)
provider_slug: uncodie
scheme_count: 2
schemes:
- description: All REST API, Workflows, and MCP requests require an API key passed as a Bearer token in the Authorization header.
  in: header
  name: bearerApiKey
  parameter: Authorization
  scheme: Bearer YOUR_API_KEY
  sources:
  - https://docs.makinari.com/rest-api
  - https://docs.makinari.com/workflows
  - https://docs.makinari.com/mcp-server/setup/remote
  type: apiKey
- description: Secure Tokens API endpoints (server-to-server secret decryption) require an API Key or Service Key via the x-api-key header.
  in: header
  name: xApiKey
  parameter: x-api-key
  sources:
  - https://docs.makinari.com/rest-api/secure-tokens
  type: apiKey
slug: uncodie-authentication
source_filename: uncodie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.makinari.com/rest-api\ndocs: https://docs.makinari.com/first-steps/api-keys\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  Makinari (formerly Uncodie) uses API-key authentication across its REST API,\n  Workflows API, Content API, and MCP server. Keys are passed as a Bearer token\n  in the Authorization header; the Secure Tokens API instead uses an x-api-key\n  header. No OAuth 2.0 or OpenID Connect authorization surface is documented.\nschemes:\n  - name: bearerApiKey\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme: 'Bearer YOUR_API_KEY'\n    description: >-\n      All REST API, Workflows, and MCP requests require an API key passed as a\n      Bearer token in the Authorization header.\n    sources:\n      - https://docs.makinari.com/rest-api\n      - https://docs.makinari.com/workflows\n      - https://docs.makinari.com/mcp-server/setup/remote\n\
  \  - name: xApiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      Secure Tokens API endpoints (server-to-server secret decryption) require\n      an API Key or Service Key via the x-api-key header.\n    sources:\n      - https://docs.makinari.com/rest-api/secure-tokens\nkey_management:\n  create: POST /api/keys\n  list: GET /api/keys?site_id=...&user_id=...\n  revoke: DELETE /api/keys?id=...&site_id=...&user_id=...\n  scopes: [read, write]\n  expiration_days_default: 90\n  docs: https://docs.makinari.com/first-steps/api-keys\n  notes: >-\n    Keys are scoped to a site and user, support optional prefix and metadata,\n    and are displayed in full only once at creation.\ncontent_api_exception:\n  description: >-\n    Content API requests from browsers succeed without an API key only when the\n    Origin header matches the domain registered for the site; server-to-server\n    requests always require a key.\n  source: https://docs.makinari.com/content-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncodie/refs/heads/main/authentication/uncodie-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- CRM
- Sales Automation
- Marketing Automation
- Lead Generation
- No Code
- MCP
---
