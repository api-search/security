---
api_key_in: []
api_specs:
- filename: cubesoftware-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/openapi/cubesoftware-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cubesoftware Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cube secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cube
provider_slug: cubesoftware
scheme_count: 1
schemes:
- code_challenge_methods_supported:
  - S256
  description: Standard Cube OAuth 2.0 flow
  flows:
  - authorizationUrl: https://portal.cubesoftware.com/o/authorize/
    flow: authorizationCode
    scopes:
    - read
    - write
    - introspection
    tokenUrl: https://api.cubesoftware.com/o/token/
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://api.cubesoftware.com/o/introspect/
  name: OAuth2
  sources:
  - openapi/cubesoftware-openapi-original.yml
  - well-known/cubesoftware-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
slug: cubesoftware-authentication
source_filename: cubesoftware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cubesoftware-openapi-original.yml\ndocs: https://api.cubesoftware.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  refresh_token: true\n  token_endpoint_auth: client_secret_basic\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.cubesoftware.com/o/authorize/\n    tokenUrl: https://api.cubesoftware.com/o/token/\n    scopes: [read, write, introspection]\n  introspection_endpoint: https://api.cubesoftware.com/o/introspect/\n  code_challenge_methods_supported: [S256]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  description: Standard Cube OAuth 2.0 flow\n  sources:\n  - openapi/cubesoftware-openapi-original.yml\n  - well-known/cubesoftware-oauth-authorization-server.json\nnotes: >-\n  Nearly\
  \ every operation additionally requires an X-Company-ID header to scope the\n  request to a specific Cube company/workspace (see conventions/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubesoftware/refs/heads/main/authentication/cubesoftware-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Spreadsheets
- SaaS
---
