---
api_key_in:
- header
api_specs:
- filename: linqalpha-openapi-original.json
  format: json
  label: LinqAlpha API
  slug: linqalpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/openapi/linqalpha-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Linqalpha Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LinqAlpha secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LinqAlpha
provider_slug: linqalpha
scheme_count: 2
schemes:
- applies_to: the whole REST API (declared as a global security requirement in the OpenAPI)
  docs: https://docs.linqalpha.com/quickstart
  example_header: 'X-API-KEY: YOUR_API_KEY'
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  primary: true
  sources:
  - openapi/linqalpha-openapi-original.json
  type: apiKey
- applies_to: the LinqAlpha MCP server at https://api.linqalpha.com/v1/mcp
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: https://api.linqalpha.com/oauth/register
  flows:
  - authorizationUrl: https://api.linqalpha.com/oauth/authorize
    flow: authorizationCode
    scopes:
      mcp:tools: Invoke the tools exposed by the LinqAlpha MCP server
    tokenUrl: https://api.linqalpha.com/oauth/token
  issuer: https://api.linqalpha.com
  name: LinqAlphaOAuth
  sources:
  - https://api.linqalpha.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: linqalpha-authentication
source_filename: linqalpha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/linqalpha-openapi-original.json\ndocs: https://docs.linqalpha.com/quickstart\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  primary: true\n  applies_to: the whole REST API (declared as a global security requirement in the OpenAPI)\n  docs: https://docs.linqalpha.com/quickstart\n  example_header: 'X-API-KEY: YOUR_API_KEY'\n  sources:\n  - openapi/linqalpha-openapi-original.json\n- name: LinqAlphaOAuth\n  type: oauth2\n  applies_to: the LinqAlpha MCP server at https://api.linqalpha.com/v1/mcp\n  issuer: https://api.linqalpha.com\n  dynamic_client_registration: https://api.linqalpha.com/oauth/register\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.linqalpha.com/oauth/authorize\n\
  \    tokenUrl: https://api.linqalpha.com/oauth/token\n    scopes:\n      mcp:tools: Invoke the tools exposed by the LinqAlpha MCP server\n  sources:\n  - https://api.linqalpha.com/.well-known/oauth-authorization-server\nnotes: >-\n  The REST API is single-factor API key auth: one X-API-KEY header applied globally, with no\n  per-operation scoping. The MCP endpoint additionally accepts an OAuth 2.0 authorization_code\n  flow with PKCE (S256) and public clients (token_endpoint_auth_methods_supported = none),\n  registered dynamically per RFC 7591. Platform-tier API keys are multi-tenant: several endpoints\n  accept an organization_id to select which organization's data the key reads, defaulting to the\n  key's primary organization.\nerrors:\n- code: API_KEY_MISSING\n  status: 401\n- code: INVALID_API_KEY\n  status: 401\ncross_references:\n  scopes: scopes/linqalpha-scopes.yml\n  conventions: conventions/linqalpha-conventions.yml\n  well_known: well-known/linqalpha-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linqalpha/refs/heads/main/authentication/linqalpha-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Financial Services
- Investment Research
- Artificial Intelligence
- Agents
- Market Data
- Equities
- Economic Data
- SEC Filings
- Retrieval Augmented Generation
- MCP
---
