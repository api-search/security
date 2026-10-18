---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hasmcp-providers-api-openapi.yml
  format: yaml
  label: HasMCP Providers API
  slug: hasmcp-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-providers-api-openapi.yml
- filename: hasmcp-servers-api-openapi.yml
  format: yaml
  label: HasMCP Servers API
  slug: hasmcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-servers-api-openapi.yml
- filename: hasmcp-variables-api-openapi.yml
  format: yaml
  label: HasMCP Variables API
  slug: hasmcp-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-variables-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Hasmcp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HasMCP secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HasMCP
provider_slug: hasmcp
scheme_count: 2
schemes:
- description: Enter 'Bearer' followed by a space and your token (e.g., 'Bearer ${HASMCP_ACCESS_TOKEN}').
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hasmcp-openapi.yaml
  type: http
- flows:
  - authorizationUrl: https://accounts.hasmcp.com/oauth2/auth
    flow: authorizationCode
    scopes: 17
    tokenUrl: https://accounts.hasmcp.com/oauth2/token
  name: oauth2
  sources:
  - openapi/hasmcp-openapi.yaml
  type: oauth2
slug: hasmcp-authentication
source_filename: hasmcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/hasmcp-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Enter 'Bearer' followed by a space and your token (e.g., 'Bearer ${HASMCP_ACCESS_TOKEN}').\n  sources:\n  - openapi/hasmcp-openapi.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.hasmcp.com/oauth2/auth\n    tokenUrl: https://accounts.hasmcp.com/oauth2/token\n    scopes: 17\n  sources:\n  - openapi/hasmcp-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/authentication/hasmcp-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- No-code
- Low-code
- MCP
- API Gateway
---
