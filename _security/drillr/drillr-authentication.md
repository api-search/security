---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: drillr-analyst-api-openapi.yml
  format: yaml
  label: drillr Public Data API Analyst API
  slug: drillr-analyst-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-analyst-api-openapi.yml
- filename: drillr-company-api-openapi.yml
  format: yaml
  label: drillr Public Data API Company API
  slug: drillr-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-company-api-openapi.yml
- filename: drillr-contract-api-openapi.yml
  format: yaml
  label: drillr Public Data API Contract API
  slug: drillr-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-contract-api-openapi.yml
- filename: drillr-earnings-api-openapi.yml
  format: yaml
  label: drillr Public Data API Earnings API
  slug: drillr-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-earnings-api-openapi.yml
- filename: drillr-events-api-openapi.yml
  format: yaml
  label: drillr Public Data API Events API
  slug: drillr-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-events-api-openapi.yml
- filename: drillr-executives-api-openapi.yml
  format: yaml
  label: drillr Public Data API Executives API
  slug: drillr-executives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-executives-api-openapi.yml
- filename: drillr-filings-api-openapi.yml
  format: yaml
  label: drillr Public Data API Filings API
  slug: drillr-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-filings-api-openapi.yml
- filename: drillr-financials-api-openapi.yml
  format: yaml
  label: drillr Public Data API Financials API
  slug: drillr-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-financials-api-openapi.yml
- filename: drillr-ownership-api-openapi.yml
  format: yaml
  label: drillr Public Data API Ownership API
  slug: drillr-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-ownership-api-openapi.yml
- filename: drillr-prices-api-openapi.yml
  format: yaml
  label: drillr Public Data API Prices API
  slug: drillr-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-prices-api-openapi.yml
- filename: drillr-signal-api-openapi.yml
  format: yaml
  label: drillr Public Data API Signal API
  slug: drillr-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/openapi/drillr-signal-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Drillr Authentication
name_suffix: Authentication
oauth_flows: []
overview: drillr Public Data API secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: drillr Public Data API
provider_slug: drillr
scheme_count: 2
schemes:
- applies_to: REST API (https://gateway.drillr.ai/api/v2)
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  provisioning: https://drillr.ai/account/api-keys
  sources:
  - openapi/drillr-openapi.json
  - https://drillr.ai/docs/quickstart
  token_prefix: drl_
  type: apiKey
- applies_to: MCP server (https://gateway.drillr.ai/mcp/data)
  authorization_endpoint: https://gateway.drillr.ai/oauth/authorize
  bearer_fallback: 'OAuth-incapable MCP clients pass the account key as Authorization: Bearer drl_...'
  client_auth: none
  dynamic_client_registration: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  name: MCP OAuth
  pkce: S256
  registration_endpoint: https://gateway.drillr.ai/oauth/register
  sources:
  - https://gateway.drillr.ai/.well-known/oauth-authorization-server
  - https://gateway.drillr.ai/.well-known/oauth-protected-resource
  - https://drillr.ai/developer/mcp-install.md
  token_endpoint: https://gateway.drillr.ai/oauth/token
  type: oauth2
slug: drillr-authentication
source_filename: drillr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://drillr.ai/docs/api\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two surfaces, two auth models. The REST API (gateway.drillr.ai/api/v2) uses a\n    static API key in the X-API-KEY header, created from the signed-in drillr\n    account. The hosted MCP server (gateway.drillr.ai/mcp/data) uses browser OAuth\n    2.0 (authorization_code + PKCE, dynamic client registration, public client) and\n    needs no key; MCP clients without OAuth support may instead pass the same\n    account key as an Authorization: Bearer header.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  applies_to: REST API (https://gateway.drillr.ai/api/v2)\n  token_prefix: drl_\n  provisioning: https://drillr.ai/account/api-keys\n  sources:\n  - openapi/drillr-openapi.json\n  - https://drillr.ai/docs/quickstart\n- name: MCP OAuth\n  type: oauth2\n  applies_to: MCP server (https://gateway.drillr.ai/mcp/data)\n\
  \  flow: authorization_code\n  pkce: S256\n  dynamic_client_registration: true\n  client_auth: none\n  authorization_endpoint: https://gateway.drillr.ai/oauth/authorize\n  token_endpoint: https://gateway.drillr.ai/oauth/token\n  registration_endpoint: https://gateway.drillr.ai/oauth/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  bearer_fallback: >-\n    OAuth-incapable MCP clients pass the account key as Authorization: Bearer drl_...\n  sources:\n  - https://gateway.drillr.ai/.well-known/oauth-authorization-server\n  - https://gateway.drillr.ai/.well-known/oauth-protected-resource\n  - https://drillr.ai/developer/mcp-install.md\ndocs: https://drillr.ai/docs/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillr/refs/heads/main/authentication/drillr-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Financial Data
- Stocks
- SEC Filings
- Fundamentals
- Earnings
- Ownership
- Corporate Events
- Analyst Ratings
- news-signals
- MCP
- agent-native
---
