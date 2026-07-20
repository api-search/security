---
api_key_in:
- header
api_specs:
- filename: heymilo-openapi-original.json
  format: json
  label: HeyMilo Public API
  slug: heymilo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Heymilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeyMilo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HeyMilo
provider_slug: heymilo
scheme_count: 2
schemes:
- description: API key for authentication. Pass your key in the X-API-KEY header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/heymilo-openapi-original.json
  type: apiKey
- applies_to: https://mcp.heymilo.ai/mcp
  description: MCP server bearer token — either an OAuth 2.1 access token (authorization_code + PKCE S256, refresh_token; scopes openid, profile, email, offline_access) or a HeyMilo API key. OAuth server metadata is published at https://mcp.heymilo.ai/.well-known/oauth-authorization-server.
  name: MCPBearer
  scheme: bearer
  sources:
  - https://docs.heymilo.ai/api-reference/mcp/getting-started
  - well-known/heymilo-oauth-authorization-server.json
  type: http
slug: heymilo-authentication
source_filename: heymilo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/heymilo-openapi-original.json\ndocs: https://docs.heymilo.ai/api-reference/public-api/documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The HeyMilo Public REST API authenticates every request with an X-API-KEY\n    header. One API key maps to one workspace, is shared per workspace, and does\n    not expire. Requests without a valid key return 401 Unauthorized. The\n    separate hosted MCP server (https://mcp.heymilo.ai/mcp) additionally accepts\n    OAuth 2.1 (Sign in with HeyMilo) or an API key, both passed as\n    Authorization: Bearer <token>.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication. Pass your key in the X-API-KEY header.\n  sources:\n  - openapi/heymilo-openapi-original.json\n- name: MCPBearer\n  type: http\n  scheme: bearer\n  applies_to: https://mcp.heymilo.ai/mcp\n  description: >-\n\
  \    MCP server bearer token — either an OAuth 2.1 access token (authorization_code\n    + PKCE S256, refresh_token; scopes openid, profile, email, offline_access) or\n    a HeyMilo API key. OAuth server metadata is published at\n    https://mcp.heymilo.ai/.well-known/oauth-authorization-server.\n  sources:\n  - https://docs.heymilo.ai/api-reference/mcp/getting-started\n  - well-known/heymilo-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/authentication/heymilo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Recruiting
- Hiring
- Human Resources
- HR Tech
- Artificial Intelligence
- AI Agents
- Interviewing
- Candidate Screening
- Voice AI
- Webhooks
- ATS Integration
---
