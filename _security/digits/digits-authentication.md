---
api_key_in: []
api_specs:
- filename: digits-openapi-original.json
  format: json
  label: Digits Connect API
  slug: digits-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/openapi/digits-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Digits Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Digits secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Digits
provider_slug: digits
scheme_count: 1
schemes:
- authorization_server_metadata: https://api.digits.com/.well-known/oauth-authorization-server
  flows:
  - authorizationUrl: https://connect.digits.com/v1/oauth/authorize
    flow: authorizationCode
    parameters:
      required:
      - client_id
      - redirect_uri
      - scope
      - state
      response_type: code
    refresh: true
    tokenUrl: https://connect.digits.com/v1/oauth/token
  metadata:
    authorization_endpoint: https://api.digits.com/oauth/authorize
    code_challenge_methods_supported:
    - S256
    grant_types_supported:
    - authorization_code
    - refresh_token
    issuer: https://api.digits.com
    registration_endpoint: https://api.digits.com/oauth/register
    revocation_endpoint: https://api.digits.com/oauth/revoke
    token_endpoint: https://api.digits.com/oauth/token
    token_endpoint_auth_methods_supported:
    - none
    - client_secret_post
    - client_secret_basic
  name: OAuth2
  type: oauth2
slug: digits-authentication
source_filename: digits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.digits.com/docs/authentication\ndocs: https://developer.digits.com/docs/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.digits.com/v1/oauth/authorize\n    tokenUrl: https://connect.digits.com/v1/oauth/token\n    refresh: true\n    parameters:\n      response_type: code\n      required: [client_id, redirect_uri, scope, state]\n  authorization_server_metadata: https://api.digits.com/.well-known/oauth-authorization-server\n  metadata:\n    issuer: https://api.digits.com\n    authorization_endpoint: https://api.digits.com/oauth/authorize\n    token_endpoint: https://api.digits.com/oauth/token\n    registration_endpoint: https://api.digits.com/oauth/register\n    revocation_endpoint: https://api.digits.com/oauth/revoke\n\
  \    code_challenge_methods_supported: [S256]\n    grant_types_supported: [authorization_code, refresh_token]\n    token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\ntoken_usage:\n  scheme: bearer\n  header: 'Authorization: Bearer <access_token>'\n  revocable: true\nnotes: >-\n  API calls are made against https://connect.digits.com/v1 with a Bearer access token obtained via the\n  authorization code grant. Note the developer-docs authorize/token endpoints are on connect.digits.com,\n  while the RFC 8414 authorization-server metadata document is published on api.digits.com; both are\n  captured above. PKCE (S256) and dynamic client registration are supported.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/authentication/digits-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- Bookkeeping
- Financial Reporting
- General Ledger
- AI
- Fintech
- Accountants
- Bill Pay
- Invoicing
---
