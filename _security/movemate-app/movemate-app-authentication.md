---
anonymous_access: false
api_key_in: []
api_specs:
- filename: movemate-app-health-api-openapi.yml
  format: yaml
  label: MoveMate Health API
  slug: movemate-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-health-api-openapi.yml
- filename: movemate-app-mcp-api-openapi.yml
  format: yaml
  label: MoveMate MCP API
  slug: movemate-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-mcp-api-openapi.yml
- filename: movemate-app-oauth-api-openapi.yml
  format: yaml
  label: MoveMate OAuth API
  slug: movemate-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/movemate-app/openapi/movemate-app-oauth-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: MoveMate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MoveMate secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MoveMate
provider_slug: movemate-app
scheme_count: 2
schemes:
- description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration (RFC 7591) at /oauth/register.
  flows:
  - authorizationUrl: https://api.movemate.app/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.movemate.app/oauth/token
  name: oauth2
  sources:
  - openapi/movemate-app-openapi.json
  type: oauth2
- description: 'Access token from the token endpoint, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/movemate-app-openapi.json
  type: http
slug: movemate-app-authentication
source_filename: movemate-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/movemate-app-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.movemate.app/oauth/authorize\n    tokenUrl: https://api.movemate.app/oauth/token\n    scopes: 4\n  description: OAuth 2.1 authorization code with PKCE S256. Dynamic client registration (RFC\n    7591) at /oauth/register.\n  sources:\n  - openapi/movemate-app-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token from the token endpoint, sent as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/movemate-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/movemate-app/authentication/movemate-app-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fitness
- Artificial Intelligence
- Workouts
- Health
- Mobile
---
