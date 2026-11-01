---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Coros Authentication
name_suffix: Authentication
oauth_flows: []
overview: COROS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: COROS
provider_slug: coros
scheme_count: 3
schemes:
- authorization_url: unknown
  description: Multi-user OAuth 2.0 credentials for established platforms
  flow: authorization_code
  name: Partner API OAuth 2.0
  scopes: []
  token_url: unknown
  type: oauth2
- authorization_url: unknown
  description: Single-user OAuth 2.0 authorization for MCP applications
  flow: authorization_code
  name: MCP OAuth 2.0
  scopes: []
  token_url: unknown
  type: oauth2
- description: Client ID and Secret issued to approved partners for API access
  field: Authorization
  in: header
  name: Client ID/Secret
  type: apiKey
slug: coros-authentication
source_filename: coros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource:\n  - https://support.coros.com/hc/en-us/articles/53181766856724-Partner-API-Access\n  - https://support.coros.com/hc/en-us/articles/53181619102996-Build-on-COROS-MCP\ndocs: https://support.coros.com/hc/en-us/articles/53181766856724-Partner-API-Access\nschemes:\n  - type: oauth2\n    name: Partner API OAuth 2.0\n    description: Multi-user OAuth 2.0 credentials for established platforms\n    flow: authorization_code\n    authorization_url: unknown\n    token_url: unknown\n    scopes: []\n  - type: oauth2\n    name: MCP OAuth 2.0\n    description: Single-user OAuth 2.0 authorization for MCP applications\n    flow: authorization_code\n    authorization_url: unknown\n    token_url: unknown\n    scopes: []\n  - type: apiKey\n    name: Client ID/Secret\n    description: Client ID and Secret issued to approved partners for API access\n    in: header\n    field: Authorization\nnote: Partner API uses OAuth 2.0 with client_id/secret\
  \ in header for webhook push notifications. MCP uses OAuth 2.0 for single-user authorization. Specific endpoints and URLs not publicly documented."
source_yaml_url: https://artifacts.apis.io/coros/authentication/coros-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Wearables
- Fitness
- GPS Watches
- Sports Technology
- Health Data
- Webhook
- Authentication
- MCP
---
