---
api_key_in: []
api_specs:
- filename: fever-reporting-api-openapi-original.json
  format: json
  label: Fever Reporting API
  slug: fever-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fever/refs/heads/main/openapi/fever-reporting-api-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fever Authentication
name_suffix: Authentication
oauth_flows:
- password
- authorization_code
overview: Fever secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and authorization_code flow(s).
provider_name: Fever
provider_slug: fever
scheme_count: 2
schemes:
- api: Fever Reporting API
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /v1/auth/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/fever-reporting-api-openapi-original.json
  type: oauth2
- api: Fever MCP / Event Catalog
  flows:
  - authorizationUrl: https://data-search.apigw.feverup.com/authorize
    flow: authorization_code
    pkce: S256
    registrationUrl: https://data-search.apigw.feverup.com/register
    scopes:
    - openid
    tokenUrl: https://data-search.apigw.feverup.com/token
  name: FeverGatewayOAuth
  sources:
  - https://data-search.apigw.feverup.com/.well-known/oauth-authorization-server
  type: oauth2
slug: fever-authentication
source_filename: fever-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fever-reporting-api-openapi-original.json\ndocs: https://developer.feverup.com/en/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  - authorization_code\n  notes: >-\n    Two distinct auth surfaces. The Reporting API uses an OAuth2 password\n    (resource-owner) flow issuing bearer tokens from POST /v1/auth/token;\n    credentials are provisioned individually by a Fever sales rep. The Fever\n    MCP / event-catalog gateway uses OAuth 2.0 authorization_code with PKCE\n    (S256) and dynamic client registration.\nschemes:\n- name: OAuth2PasswordBearer\n  api: Fever Reporting API\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /v1/auth/token\n    scopes: 0\n  sources:\n  - openapi/fever-reporting-api-openapi-original.json\n- name: FeverGatewayOAuth\n  api: Fever MCP / Event Catalog\n  type: oauth2\n  flows:\n  - flow: authorization_code\n    pkce: S256\n    authorizationUrl: https://data-search.apigw.feverup.com/authorize\n\
  \    tokenUrl: https://data-search.apigw.feverup.com/token\n    registrationUrl: https://data-search.apigw.feverup.com/register\n    scopes: [openid]\n  sources:\n  - https://data-search.apigw.feverup.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fever/refs/heads/main/authentication/fever-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Consumer
- Live Entertainment
- Events
- Ticketing
- Experiences
- Reporting
- MCP
---
