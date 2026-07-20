---
api_key_in: []
auth_types:
- apiKey
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Horizon3Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Horizon3.ai secures its APIs with apiKey, http-bearer, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Horizon3.ai
provider_slug: horizon3ai
scheme_count: 3
schemes:
- auth_endpoints:
  - region: US
    url: https://api.gateway.horizon3ai.com/v1/auth
  - region: EU
    url: https://api.gateway.horizon3ai.eu/v1/auth
  description: 'An API key generated in the Portal (User -> Account Settings). It is POSTed as JSON {"key": "<H3_API_KEY>"} to the regional /v1/auth endpoint and exchanged for a short-lived JWT. The key itself is not sent on GraphQL requests.'
  name: apiKeyAuth
  roles:
  - description: Basic read/write; can run pentests and read results.
    name: User
  - description: Can read pentest results but cannot run pentests.
    name: Read-only
  - description: Specialized, heavily restricted role for NodeZero Runners.
    name: NodeZero Runner
  type: apiKey
- applied_to: https://api.gateway.horizon3ai.com/v1/graphql
  bearerFormat: JWT
  description: 'The JWT returned by /v1/auth is sent as an Authorization: Bearer header on every GraphQL request to /v1/graphql. Expires after 1 hour; re-authenticate to renew.'
  name: bearerAuth
  scheme: bearer
  type: http
- authorizationUrl: https://oauth-proxy.horizon3ai.com/authorize
  description: The Horizon3.ai-hosted MCP server authenticates with OAuth 2.1 + PKCE via oauth-proxy.horizon3ai.com (scopes read, write). See mcp/horizon3ai-mcp.yml.
  flow: authorizationCode
  name: oauth2Mcp
  scopes:
  - read
  - write
  tokenUrl: https://oauth-proxy.horizon3ai.com/token
  type: oauth2
slug: horizon3ai-authentication
source_filename: horizon3ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.horizon3.ai/api/getting_started/authenticate/\ndocs: https://docs.horizon3.ai/api/getting_started/authenticate/\nsummary:\n  types: [apiKey, http-bearer, oauth2]\n  api_key_exchange: true\n  bearer_format: JWT\n  token_ttl_seconds: 3600\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  description: >-\n    An API key generated in the Portal (User -> Account Settings). It is POSTed as\n    JSON {\"key\": \"<H3_API_KEY>\"} to the regional /v1/auth endpoint and exchanged for\n    a short-lived JWT. The key itself is not sent on GraphQL requests.\n  auth_endpoints:\n  - region: US\n    url: https://api.gateway.horizon3ai.com/v1/auth\n  - region: EU\n    url: https://api.gateway.horizon3ai.eu/v1/auth\n  roles:\n  - name: User\n    description: Basic read/write; can run pentests and read results.\n  - name: Read-only\n    description: Can read pentest results but cannot run pentests.\n  - name: NodeZero Runner\n    description:\
  \ Specialized, heavily restricted role for NodeZero Runners.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    The JWT returned by /v1/auth is sent as an Authorization: Bearer header on every\n    GraphQL request to /v1/graphql. Expires after 1 hour; re-authenticate to renew.\n  applied_to: https://api.gateway.horizon3ai.com/v1/graphql\n- name: oauth2Mcp\n  type: oauth2\n  description: >-\n    The Horizon3.ai-hosted MCP server authenticates with OAuth 2.1 + PKCE via\n    oauth-proxy.horizon3ai.com (scopes read, write). See mcp/horizon3ai-mcp.yml.\n  flow: authorizationCode\n  authorizationUrl: https://oauth-proxy.horizon3ai.com/authorize\n  tokenUrl: https://oauth-proxy.horizon3ai.com/token\n  scopes: [read, write]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon3ai/refs/heads/main/authentication/horizon3ai-authentication.yml
summary_line: apiKey/http-bearer/oauth2 · 3 schemes
tags:
- Company
- Security
- Cybersecurity
- Penetration Testing
- Autonomous Pentesting
- Attack Surface Management
- Exposure Management
- Vulnerability Management
- GraphQL
- Offensive Security
---
