---
api_key_in:
- header
api_specs:
- filename: alterestate-openapi.yml
  format: yaml
  label: AlterEstate API
  slug: alterestate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/openapi/alterestate-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alterestate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AlterEstate secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AlterEstate
provider_slug: alterestate
scheme_count: 3
schemes:
- description: Public API token from the AlterEstate dashboard (Settings > Public API Token, admin access). Used for read endpoints.
  in: header
  name: aetoken
  parameter: aetoken
  sources:
  - openapi/alterestate-openapi.yml
  type: apiKey
- description: 'Account API key sent as: Authorization: Token <api_key>. Used for lead submission.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/alterestate-openapi.yml
  type: apiKey
- description: OAuth 2.0 authorization used by the AlterEstate (Brik/alterai) hosted MCP server.
  flows:
  - authorizationUrl: https://secure.alterestate.com/oauth/authorize/
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://secure.alterestate.com/oauth/token/
  name: oauth2
  sources:
  - openapi/alterestate-openapi.yml
  type: oauth2
slug: alterestate-authentication
source_filename: alterestate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/alterestate-openapi.yml\ndocs: https://dev.alterestate.com/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: aetoken\n  type: apiKey\n  in: header\n  parameter: aetoken\n  description: Public API token from the AlterEstate dashboard (Settings > Public API Token,\n    admin access). Used for read endpoints.\n  sources:\n  - openapi/alterestate-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Account API key sent as: Authorization: Token <api_key>. Used for lead submission.'\n  sources:\n  - openapi/alterestate-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.alterestate.com/oauth/authorize/\n    tokenUrl: https://secure.alterestate.com/oauth/token/\n    scopes: 1\n  description: OAuth 2.0 authorization used by\
  \ the AlterEstate (Brik/alterai) hosted MCP server.\n  sources:\n  - openapi/alterestate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/authentication/alterestate-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Real Estate
- CRM
- Property Management
- Lead Management
- Latin America
- SaaS
- Artificial Intelligence
- MCP
---
