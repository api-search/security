---
api_key_in: []
auth_types:
- oauth2
description: 'The Butlr API is protected with OAuth 2.0 bearer tokens issued by Auth0. Two grant types are supported: the Password grant (for user-context access, returns access_token + refresh_token + id_token) and the Client Credentials grant (machine-to-machine, for server-to-server access using a Client ID and Client Secret minted from the Butlr Web App API tokens tab). Tokens are presented as `Authorization: Bearer <access_token>` on subsequent GraphQL and Reporting API calls. The official MCP server uses the client credentials grant.'
kind: authentication
layout: security
method: searched
name: Butlr Technologies Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: Butlr Technologies secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: Butlr Technologies
provider_slug: butlr-technologies
scheme_count: 2
schemes:
- flow: password
  name: OAuth2PasswordGrant
  request_body:
    password: null
    username: null
  returns:
  - access_token
  - refresh_token
  - id_token
  - scope
  - expires_in
  - token_type
  source: docs
  token_endpoint: https://api.butlr.io/api/v2/login
  token_type: Bearer
  type: oauth2
- audience: https://butlrauth/
  credential_minting: https://app.butlr.io
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request_body:
    audience: null
    client_id: null
    client_secret: null
    grant_type: client_credentials
  returns:
  - access_token
  - scope
  - expires_in
  - token_type
  source: docs
  token_endpoint: https://api.butlr.io/api/v2/clients/login
  token_type: Bearer
  type: oauth2
slug: butlr-technologies-authentication
source_filename: butlr-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.butlr.io/getting-started/authentication.md\ndocs: https://docs.butlr.io/getting-started/authentication.md\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [password, clientCredentials]\n  identity_provider: Auth0\ndescription: >-\n  The Butlr API is protected with OAuth 2.0 bearer tokens issued by Auth0. Two\n  grant types are supported: the Password grant (for user-context access,\n  returns access_token + refresh_token + id_token) and the Client Credentials\n  grant (machine-to-machine, for server-to-server access using a Client ID and\n  Client Secret minted from the Butlr Web App API tokens tab). Tokens are\n  presented as `Authorization: Bearer <access_token>` on subsequent GraphQL and\n  Reporting API calls. The official MCP server uses the client credentials grant.\nschemes:\n  - name: OAuth2PasswordGrant\n    type: oauth2\n    flow: password\n    token_endpoint: https://api.butlr.io/api/v2/login\n\
  \    request_body: { username, password }\n    returns: [access_token, refresh_token, id_token, scope, expires_in, token_type]\n    token_type: Bearer\n    source: docs\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://api.butlr.io/api/v2/clients/login\n    audience: https://butlrauth/\n    request_body: { client_id, client_secret, audience, grant_type: client_credentials }\n    returns: [access_token, scope, expires_in, token_type]\n    token_type: Bearer\n    credential_minting: https://app.butlr.io  # Account Settings -> API tokens -> Create token\n    source: docs\nnotes:\n  - Client credentials are the recommended path for server-to-server and agent (MCP) integrations.\n  - Client ID and Client Secret are shown once at creation and cannot be retrieved again.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butlr-technologies/refs/heads/main/authentication/butlr-technologies-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Occupancy Sensing
- People Counting
- Smart Buildings
- Space Utilization
- IoT
- Thermal Sensors
- Real-Time Data
- GraphQL
- Webhooks
---
