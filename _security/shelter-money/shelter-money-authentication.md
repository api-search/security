---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shelter Money Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shelter declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Shelter
provider_slug: shelter-money
scheme_count: 1
schemes:
- description: Scoped Shelter API key, created and revoked at https://shelter.money/developer. Keys are read-only by default, prefixed wv_, stored by Shelter as SHA-256 hashes at rest, and shown only once at creation (only the prefix displays afterward). In the official MCP server the key is supplied via the SHELTER_API_KEY environment variable and sent as the X-Shelter-Key request header (per the published client source, src/client.ts).
  in: header
  name: X-Shelter-Key
  type: apiKey
slug: shelter-money-authentication
source_filename: shelter-money-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://shelter.money/developers\ndocs: https://shelter.money/developers\nschemes:\n- type: apiKey\n  in: header\n  name: X-Shelter-Key\n  description: >-\n    Scoped Shelter API key, created and revoked at https://shelter.money/developer. Keys are\n    read-only by default, prefixed wv_, stored by Shelter as SHA-256 hashes at rest, and shown\n    only once at creation (only the prefix displays afterward). In the official MCP server the\n    key is supplied via the SHELTER_API_KEY environment variable and sent as the X-Shelter-Key\n    request header (per the published client source, src/client.ts).\nnotes:\n- No OAuth flows, OpenID Connect, or mutual TLS are documented; API keys are the only scheme.\n- End-user identity comes solely from the scoped key; the MCP package holds no Plaid tokens or\n  bank credentials.\n- Without a key the official MCP server fails closed — tool definitions load but every response\n  is suppressed\
  \ with reasonCodes [MISSING_SHELTER_API_KEY] and no financial values.\nevidence:\n- url: https://shelter.money/developers\n  status: 200\n- url: https://raw.githubusercontent.com/nextauralabs/shelter-mcp/main/src/client.ts\n  status: 200\n- url: https://raw.githubusercontent.com/nextauralabs/shelter-mcp/main/SECURITY.md\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shelter-money/refs/heads/main/authentication/shelter-money-authentication.yml
summary_line: 1 scheme
tags:
- Personal Finance
- Budgeting
- Fintech
- MCP
- AI Agents
- Cash Flow Forecasting
---
