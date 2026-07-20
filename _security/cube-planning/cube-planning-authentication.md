---
api_key_in: []
api_specs:
- filename: cube-planning-openapi-original.yml
  format: yaml
  label: Cube API
  slug: cube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/openapi/cube-planning-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cube Planning Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cube Planning secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cube Planning
provider_slug: cube-planning
scheme_count: 1
schemes:
- description: Standard Cube OAuth 2.0 flow
  flows:
  - authorizationUrl: https://portal.cubesoftware.com/o/authorize/
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://api.cubesoftware.com/o/introspect/
    pkce: S256
    scopes:
    - read
    - write
    - introspection
    tokenUrl: https://api.cubesoftware.com/o/token/
    token_endpoint_auth: client_secret_basic
  name: OAuth2
  sources:
  - openapi/cube-planning-openapi-original.yml
  - well-known/cube-planning-oauth-authorization-server.json
  type: oauth2
slug: cube-planning-authentication
source_filename: cube-planning-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cube-planning-openapi-original.yml\ndocs: https://www.cubesoftware.com/developer-center\nwell_known: https://api.cubesoftware.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Cube's API uses OAuth 2.0 authorization-code with PKCE (S256). Access tokens are\n    Bearer tokens sent in the Authorization header. Refresh tokens are supported. A\n    required X-Company-ID header scopes most requests to a specific Cube company/tenant,\n    and an Accept header carries the API version (e.g. `Accept: application/json; version=1.0`).\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.cubesoftware.com/o/authorize/\n    tokenUrl: https://api.cubesoftware.com/o/token/\n    introspectionUrl: https://api.cubesoftware.com/o/introspect/\n    pkce: S256\n    grant_types: [authorization_code,\
  \ refresh_token]\n    token_endpoint_auth: client_secret_basic\n    scopes: [read, write, introspection]\n  description: Standard Cube OAuth 2.0 flow\n  sources:\n  - openapi/cube-planning-openapi-original.yml\n  - well-known/cube-planning-oauth-authorization-server.json\ntenant_header:\n  name: X-Company-ID\n  in: header\n  required: true\n  applies_to_operations: 226\n  description: Identifies the Cube company/tenant a request operates against.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cube-planning/refs/heads/main/authentication/cube-planning-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- Analytics
- Planning
---
