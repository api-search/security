---
api_key_in:
- header
api_specs:
- filename: charthop-openapi-original.json
  format: json
  label: ChartHop REST API
  slug: charthop-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/openapi/charthop-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Charthop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Charthop secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Charthop
provider_slug: charthop
scheme_count: 2
schemes:
- description: Server-to-server apps are issued an API authorization token when ChartHop creates and installs the app in an org account. The token is presented as an Authorization Bearer header and acts on behalf of the app (a special user with scoped permissions). Apps are requested via support@charthop.com ("new app request").
  docs: https://docs.charthop.com/developer-basics
  name: appAuthorizationToken
  scheme: bearer
  type: http
- authorizationUrl: https://app.charthop.com/oauth/mcp/authorize
  description: OAuth 2.1 authorization-code + PKCE flow used to authorize agent MCP sessions and OAuth apps. Supports dynamic client registration via client-id metadata documents.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  pkce: S256
  source: well-known/charthop-oauth-authorization-server.json
  tokenUrl: https://api.charthop.com/oauth/token
  type: oauth2
slug: charthop-authentication
source_filename: charthop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.charthop.com/swagger.json\ndocs: https://docs.charthop.com/developer-basics\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    The published Swagger 2.0 document declares no securityDefinitions; the auth model\n    below is captured from ChartHop's developer documentation and its live OAuth\n    authorization-server metadata (well-known/charthop-oauth-authorization-server.json).\nschemes:\n- name: appAuthorizationToken\n  type: http\n  scheme: bearer\n  description: >-\n    Server-to-server apps are issued an API authorization token when ChartHop creates\n    and installs the app in an org account. The token is presented as an Authorization\n    Bearer header and acts on behalf of the app (a special user with scoped permissions).\n    Apps are requested via support@charthop.com (\"new app request\").\n  docs: https://docs.charthop.com/developer-basics\n\
  - name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    OAuth 2.1 authorization-code + PKCE flow used to authorize agent MCP sessions and\n    OAuth apps. Supports dynamic client registration via client-id metadata documents.\n  authorizationUrl: https://app.charthop.com/oauth/mcp/authorize\n  tokenUrl: https://api.charthop.com/oauth/token\n  pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  source: well-known/charthop-oauth-authorization-server.json\npermissions_model: >-\n  Apps declare required permission levels at request time; access is governed by\n  ChartHop's user-role permission system rather than named OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/authentication/charthop-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- HR
- People Analytics
- HRIS
- Workforce Planning
- Compensation
- Human Resources
- Org Chart
- MCP
---
