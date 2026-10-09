---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: akta-pro-company-api-openapi.yml
  format: yaml
  label: akta.pro Company API
  slug: akta-pro-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-company-api-openapi.yml
- filename: akta-pro-list-generation-api-openapi.yml
  format: yaml
  label: akta.pro List Generation API
  slug: akta-pro-list-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-list-generation-api-openapi.yml
- filename: akta-pro-news-api-openapi.yml
  format: yaml
  label: akta.pro News API
  slug: akta-pro-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-news-api-openapi.yml
- filename: akta-pro-reviews-api-openapi.yml
  format: yaml
  label: akta.pro Reviews API
  slug: akta-pro-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-reviews-api-openapi.yml
- filename: akta-pro-supporting-apis-api-openapi.yml
  format: yaml
  label: akta.pro Supporting APIs API
  slug: akta-pro-supporting-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/openapi/akta-pro-supporting-apis-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Akta Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: akta.pro secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: akta.pro
provider_slug: akta-pro
scheme_count: 2
schemes:
- description: API key obtained from your Akta account.
  docs: https://docs.akta.pro/getting-started/overview
  example: 'curl -G "https://api.akta.pro/api/v1/company/search/?query=canva" -H "x-api-key: YOUR_API_KEY"'
  in: header
  key_management: Generate in the Playground (https://playground.akta.pro/dashboard/manage/api-keys); "The API key is shown once."
  key_prefix: wk_
  name: xApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/akta-pro-openapi.yml
  type: apiKey
  unauthenticated_response: 401 application/json (probed 2026-10-07)
- alternative: x-api-key header on the MCP request (Cursor / VS Code / Claude Code / OpenCode configs in the setup docs)
  dynamic_client_registration: https://mcp.akta.pro/register
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.akta.pro/authorize
      refreshUrl: https://mcp.akta.pro/token
      scopes: {}
      tokenUrl: https://mcp.akta.pro/token
  name: mcpOAuth
  pkce: S256
  protected_resource_metadata: https://mcp.akta.pro/.well-known/oauth-protected-resource/mcp
  scope: MCP server https://mcp.akta.pro/mcp only
  sources:
  - https://mcp.akta.pro/.well-known/oauth-authorization-server
  - https://docs.akta.pro/docs/developer-tools/mcp/setup.md
  type: oauth2
slug: akta-pro-authentication
source_filename: akta-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: openapi/akta-pro-openapi.yml; https://docs.akta.pro/getting-started/overview.md; https://docs.akta.pro/docs/developer-tools/mcp/setup.md;\n  https://mcp.akta.pro/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: 'REST API: x-api-key only. MCP server: OAuth 2.1 (authorization code + PKCE, DCR, no scopes published) or\n    x-api-key header.'\nschemes:\n- name: xApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key obtained from your Akta account.\n  sources:\n  - openapi/akta-pro-openapi.yml\n  docs: https://docs.akta.pro/getting-started/overview\n  key_prefix: wk_\n  key_management: Generate in the Playground (https://playground.akta.pro/dashboard/manage/api-keys); \"The API key\n    is shown once.\"\n  example: 'curl -G \"https://api.akta.pro/api/v1/company/search/?query=canva\" -H \"x-api-key: YOUR_API_KEY\"'\n  unauthenticated_response:\
  \ 401 application/json (probed 2026-10-07)\n- name: mcpOAuth\n  type: oauth2\n  scope: MCP server https://mcp.akta.pro/mcp only\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.akta.pro/authorize\n      tokenUrl: https://mcp.akta.pro/token\n      refreshUrl: https://mcp.akta.pro/token\n      scopes: {}\n  pkce: S256\n  dynamic_client_registration: https://mcp.akta.pro/register\n  protected_resource_metadata: https://mcp.akta.pro/.well-known/oauth-protected-resource/mcp\n  alternative: x-api-key header on the MCP request (Cursor / VS Code / Claude Code / OpenCode configs in the setup\n    docs)\n  sources:\n  - https://mcp.akta.pro/.well-known/oauth-authorization-server\n  - https://docs.akta.pro/docs/developer-tools/mcp/setup.md\ndocs: https://docs.akta.pro/getting-started/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akta-pro/refs/heads/main/authentication/akta-pro-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Company Data
- Company Intelligence
- News
- Alternative Data
- Private Companies
- Firmographics
- Data Enrichment
- Signals
- MCP
- Market Intelligence
---
