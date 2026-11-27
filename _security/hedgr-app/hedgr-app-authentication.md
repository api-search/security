---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hedgr-app-health-api-openapi.yml
  format: yaml
  label: HEDGR Health API
  slug: hedgr-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-health-api-openapi.yml
- filename: hedgr-app-mcp-api-openapi.yml
  format: yaml
  label: HEDGR MCP API
  slug: hedgr-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-mcp-api-openapi.yml
- filename: hedgr-app-oauth-discovery-api-openapi.yml
  format: yaml
  label: HEDGR OAuth discovery API
  slug: hedgr-app-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-oauth-discovery-api-openapi.yml
- filename: hedgr-app-partner-api-api-openapi.yml
  format: yaml
  label: HEDGR Partner API
  slug: hedgr-app-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-partner-api-api-openapi.yml
- filename: hedgr-app-rates-api-openapi.yml
  format: yaml
  label: HEDGR Rates API
  slug: hedgr-app-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-rates-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: HEDGR Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HEDGR secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HEDGR
provider_slug: hedgr-app
scheme_count: 2
schemes:
- description: OAuth 2.1 authorization-code flow with PKCE and dynamic client registration. See /.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://hedgr.app/mcp/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://hedgr.app/mcp/oauth/token
  name: mcpOAuth
  sources:
  - openapi/hedgr-app-openapi.json
  type: oauth2
- bearerFormat: hpk_live_...
  description: 'Partner API key issued by Hedgr to a broker firm. Send as Authorization: Bearer <key>. See https://hedgr.app/partner-api.'
  name: partnerKey
  scheme: bearer
  sources:
  - openapi/hedgr-app-openapi.json
  type: http
slug: hedgr-app-authentication
source_filename: hedgr-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hedgr-app-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hedgr.app/mcp/oauth/authorize\n    tokenUrl: https://hedgr.app/mcp/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization-code flow with PKCE and dynamic client registration.\n    See /.well-known/oauth-authorization-server.\n  sources:\n  - openapi/hedgr-app-openapi.json\n- name: partnerKey\n  type: http\n  scheme: bearer\n  bearerFormat: hpk_live_...\n  description: 'Partner API key issued by Hedgr to a broker firm. Send as Authorization: Bearer\n    <key>. See https://hedgr.app/partner-api.'\n  sources:\n  - openapi/hedgr-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hedgr-app/authentication/hedgr-app-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Finance
- Artificial Intelligence
- Foreign Exchange
- Small Business
- Accounting
- Platform
---
