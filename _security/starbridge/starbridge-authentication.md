---
api_key_in: []
api_specs:
- filename: starbridge-openapi.json
  format: json
  label: Starbridge External Public API
  slug: starbridge-external-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Starbridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Starbridge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Starbridge
provider_slug: starbridge
scheme_count: 1
schemes:
- description: 'HTTP Bearer authentication. Create an API key in the Starbridge dashboard (Settings -> API Keys, https://dashboard.starbridge.ai/settings/api-keys) and send it as ''Authorization: Bearer <api_key>''. Keys are named per service/integration.'
  issuance_url: https://dashboard.starbridge.ai/settings/api-keys
  name: apiKey
  scheme: bearer
  sources:
  - openapi/starbridge-openapi.json
  - https://hc.starbridge.ai/api-reference/rest/generating-an-api-key
  type: http
slug: starbridge-authentication
source_filename: starbridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://hc.starbridge.ai/api-reference/rest/generating-an-api-key +\n  openapi/starbridge-openapi.json\ndocs: https://hc.starbridge.ai/api-reference/rest/generating-an-api-key\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: >-\n    HTTP Bearer authentication. Create an API key in the Starbridge dashboard\n    (Settings -> API Keys, https://dashboard.starbridge.ai/settings/api-keys) and\n    send it as 'Authorization: Bearer <api_key>'. Keys are named per service/integration.\n  issuance_url: https://dashboard.starbridge.ai/settings/api-keys\n  sources:\n  - openapi/starbridge-openapi.json\n  - https://hc.starbridge.ai/api-reference/rest/generating-an-api-key\n# MCP access uses a separate OAuth 2.0 flow (auth.starbridge.ai); see mcp/starbridge-mcp.yml.\nmcp_auth:\n  type: oauth2\n  authorization_server: https://auth.starbridge.ai\n  scopes: [mcp:tools]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/authentication/starbridge-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Sales Intelligence
- Go To Market
- Public Sector
- Education
- Government
- Procurement
- Buyer Intelligence
- MCP
---
