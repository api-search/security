---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Butlr Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
- authorizationCode
overview: Butlr secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, clientCredentials, and authorizationCode flow(s).
provider_name: Butlr
provider_slug: butlr
scheme_count: 3
schemes:
- flow: password
  name: OAuth2 Password Grant
  request: POST JSON {username, password}
  returns:
  - access_token
  - refresh_token
  - id_token
  - scope
  - expires_in
  - token_type
  token_endpoint: https://api.butlr.io/api/v2/login
  token_type: Bearer
  type: oauth2
  use_case: First-party/trusted clients acting on behalf of a specific user; issues refresh tokens for seamless session maintenance.
- audience: https://butlrauth/
  flow: clientCredentials
  name: OAuth2 Client Credentials Grant
  provisioning: Mint client credentials in the Butlr Web App (app.butlr.io) under Account Settings > API tokens, or programmatically via the Auth0 M2M Client Service (POST /api/v1/client). Credentials are authorized for the Butlr API audience (https://butlrauth/).
  type: oauth2
  use_case: Server-to-server / machine-to-machine access using client_id + client_secret, with no end-user context. Recommended for API integrations and the MCP server.
- flow: authorizationCode
  name: OAuth2 Authorization Code Grant
  provider: Auth0 (hosted redirect)
  type: oauth2
  use_case: Used by the Butlr Dashboard to keep Butlr out of the password-exchange flow. Documented as planned for the developer API but not yet exposed there.
slug: butlr-authentication
source_filename: butlr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.butlr.io/getting-started/authentication\ndocs: https://docs.butlr.io/getting-started\nsummary:\n  types: [oauth2]\n  bearer: true\n  token_format: JWT\n  identity_provider: Auth0\n  oauth2_flows: [password, clientCredentials, authorizationCode]\nschemes:\n- name: OAuth2 Password Grant\n  type: oauth2\n  flow: password\n  token_endpoint: https://api.butlr.io/api/v2/login\n  request: 'POST JSON {username, password}'\n  returns: [access_token, refresh_token, id_token, scope, expires_in, token_type]\n  token_type: Bearer\n  use_case: >-\n    First-party/trusted clients acting on behalf of a specific user; issues\n    refresh tokens for seamless session maintenance.\n- name: OAuth2 Client Credentials Grant\n  type: oauth2\n  flow: clientCredentials\n  audience: https://butlrauth/\n  use_case: >-\n    Server-to-server / machine-to-machine access using client_id + client_secret,\n    with no end-user context. Recommended\
  \ for API integrations and the MCP server.\n  provisioning: >-\n    Mint client credentials in the Butlr Web App (app.butlr.io) under Account\n    Settings > API tokens, or programmatically via the Auth0 M2M Client Service\n    (POST /api/v1/client). Credentials are authorized for the Butlr API audience\n    (https://butlrauth/).\n- name: OAuth2 Authorization Code Grant\n  type: oauth2\n  flow: authorizationCode\n  provider: Auth0 (hosted redirect)\n  use_case: >-\n    Used by the Butlr Dashboard to keep Butlr out of the password-exchange flow.\n    Documented as planned for the developer API but not yet exposed there.\nusage:\n  header: 'Authorization: Bearer <access_token>'\nnotes: >-\n  All API requests are authenticated with OAuth 2.0-compliant JWT access tokens\n  passed as a Bearer token. Identity is backed by Auth0. There is no API-key\n  scheme. Legacy v2 password-grant login endpoint remains at /api/v2/login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butlr/refs/heads/main/authentication/butlr-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Sensors
- Occupancy
- People Sensing
- Smart Buildings
- Spatial Intelligence
- IoT
- GraphQL
- Webhooks
- Real Estate
---
