---
api_key_in:
- header
api_specs:
- filename: rentahuman-openapi-original.yml
  format: yaml
  label: RentAHuman.ai API
  slug: rentahumanai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentahuman/refs/heads/main/openapi/rentahuman-openapi-original.yml
auth_types:
- apiKey
- http
- firebase
- mcp-identity
description: ''
kind: authentication
layout: security
method: searched
name: Rentahuman Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rentahuman secures its APIs with apiKey, http, firebase, and mcp-identity across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rentahuman
provider_slug: rentahuman
scheme_count: 4
schemes:
- docs: https://rentahuman.ai/api-docs
  format: rah_live_... (also rah_YOUR_API_KEY)
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  type: apiKey
- docs: https://rentahuman.ai/api-docs
  format: Bearer rah_live_...
  name: BearerToken
  parameter: Authorization
  scheme: bearer
  type: http
- description: Firebase account authentication for protected/session endpoints.
  docs: https://rentahuman.ai/docs
  name: FirebaseSession
  type: firebase
- description: Ed25519-backed MCP cryptographic identity, bound via POST /api/keys/register-identity.
  docs: https://rentahuman.ai/docs
  name: McpIdentity
  type: mcp-identity
slug: rentahuman-authentication
source_filename: rentahuman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://rentahuman.ai/api-docs\ndocs: https://rentahuman.ai/docs\nsummary:\n  types: [apiKey, http, firebase, mcp-identity]\n  api_key_in: [header]\n  notes: >-\n    The published OpenAPI declares no securitySchemes; the auth model is\n    documented in the developer docs and captured here (method: searched).\nschemes:\n  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    format: rah_live_... (also rah_YOUR_API_KEY)\n    docs: https://rentahuman.ai/api-docs\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    format: Bearer rah_live_...\n    docs: https://rentahuman.ai/api-docs\n  - name: FirebaseSession\n    type: firebase\n    description: Firebase account authentication for protected/session endpoints.\n    docs: https://rentahuman.ai/docs\n  - name: McpIdentity\n    type: mcp-identity\n    description: Ed25519-backed MCP cryptographic identity,\
  \ bound via POST /api/keys/register-identity.\n    docs: https://rentahuman.ai/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentahuman/refs/heads/main/authentication/rentahuman-authentication.yml
summary_line: apiKey/http/firebase/mcp-identity · 4 schemes
tags:
- Company
- Marketplace
- AI Agents
- Human-in-the-Loop
- Gig Economy
- MCP
- Labor
- Payments
---
