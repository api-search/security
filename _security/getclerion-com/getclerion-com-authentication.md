---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getclerion-com-deploys-api-openapi.yml
  format: yaml
  label: Clerion Deploys API
  slug: getclerion-com-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-deploys-api-openapi.yml
- filename: getclerion-com-discovery-api-openapi.yml
  format: yaml
  label: Clerion Discovery API
  slug: getclerion-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-discovery-api-openapi.yml
- filename: getclerion-com-mcp-api-openapi.yml
  format: yaml
  label: Clerion MCP API
  slug: getclerion-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-mcp-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Clerion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clerion secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clerion
provider_slug: getclerion-com
scheme_count: 2
schemes:
- description: The account key from the dashboard, under Your model. Replacing the key there revokes it everywhere.
  name: clerionKey
  scheme: bearer
  sources:
  - openapi/getclerion-com-openapi.json
  type: http
- description: 'OAuth 2.1 for MCP clients: authorization code with PKCE, dynamic client registration at /oauth/register. Discover it at /.well-known/oauth-authorization-server.'
  flows:
  - authorizationUrl: https://api.getclerion.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.getclerion.com/oauth/token
  name: oauth
  sources:
  - openapi/getclerion-com-openapi.json
  type: oauth2
slug: getclerion-com-authentication
source_filename: getclerion-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/getclerion-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: clerionKey\n  type: http\n  scheme: bearer\n  description: The account key from the dashboard, under Your model. Replacing the key there\n    revokes it everywhere.\n  sources:\n  - openapi/getclerion-com-openapi.json\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getclerion.com/oauth/authorize\n    tokenUrl: https://api.getclerion.com/oauth/token\n    scopes: 1\n  description: 'OAuth 2.1 for MCP clients: authorization code with PKCE, dynamic client registration\n    at /oauth/register. Discover it at /.well-known/oauth-authorization-server.'\n  sources:\n  - openapi/getclerion-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getclerion-com/authentication/getclerion-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Analytics
- Website Intelligence
- Founders
- Marketing
---
