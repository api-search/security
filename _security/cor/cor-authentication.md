---
api_key_in: []
api_specs:
- filename: cor-openapi.json
  format: json
  label: COR API
  slug: cor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/openapi/cor-openapi.json
- filename: cor-resource-allocation-openapi.json
  format: json
  label: COR Resource Allocation API
  slug: cor-resource-allocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/openapi/cor-resource-allocation-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cor Authentication
name_suffix: Authentication
oauth_flows: []
overview: COR secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: COR
provider_slug: cor
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: All COR API requests are authorized with a JWT bearer token obtained from the OAuth token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cor-openapi.json
  - openapi/cor-resource-allocation-openapi.json
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/cor-openapi.json
  type: http
slug: cor-authentication
source_filename: cor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cor-openapi.json, openapi/cor-resource-allocation-openapi.json, https://developers.projectcor.com/api-reference/auth/jwt-authorization-by-client-credentials\ndocs: https://developers.projectcor.com/api-reference/auth/jwt-authorization-by-client-credentials\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: OAuth 2.0 issuing JWT bearer tokens\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: All COR API requests are authorized with a JWT bearer token obtained\n    from the OAuth token endpoint.\n  sources:\n  - openapi/cor-openapi.json\n  - openapi/cor-resource-allocation-openapi.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cor-openapi.json\noauth2:\n  token_url: https://api.projectcor.com/v1/oauth/token\n  alternate_token_url: https://api.projectcor.com/v1/oauth2/token\n  refresh_url: https://api.projectcor.com/v1/oauth/refreshtoken\n\
  \  grant_types:\n  - client_credentials\n  - authorization_code\n  - password\n  - refresh_token\n  token_format: JWT\n  response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  - refresh_token\n  scopes: []\n  scopes_note: The COR API does not declare granular OAuth scopes; access is governed\n    by the authenticated user's workspace role/permissions.\nnotes:\n- COR documents four JWT authorization flows (authorization code, client credentials,\n  user credentials, refresh token) plus a GET /me endpoint to resolve the authenticated\n  user.\n- The hosted MCP server (mcp.projectcor.com) authenticates with OAuth 2.0 over\n  Streamable HTTP.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cor/refs/heads/main/authentication/cor-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Agency Management
- Project Management
- Time Tracking
- Profitability
- Resource Allocation
- Professional Services
- MCP
---
