---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Aspire Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Aspire secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Aspire
provider_slug: aspire
scheme_count: 2
schemes:
- description: Server-to-server access to your own Aspire account. Obtain a Client ID and Client Secret from the Aspire dashboard, then exchange them for an access token via POST https://api.aspireapp.com/public/v1/login. Tokens expire in 900 seconds; no refresh token is issued.
  flow: clientCredentials
  name: ClientCredentials
  source: https://docs.api.aspireapp.com/authentication
  tokenUrl: https://api.aspireapp.com/public/v1/login
  type: oauth2
- description: Third-party apps acting on another user's Aspire data with their consent. Register the app with the Aspire Account Manager to receive a Client ID and Client Secret, redirect the user to the authorization URL, exchange the returned authorization code for an access token plus refresh token, and use the refresh token to mint fresh access tokens.
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  pkce: true
  source: https://docs.api.aspireapp.com/authentication
  type: oauth2
slug: aspire-authentication
source_filename: aspire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.api.aspireapp.com/authentication\ndocs: https://docs.api.aspireapp.com/authentication\napi: Aspire API\nsummary:\n  types: [oauth2, http]\n  token_type: bearer\n  header: Authorization\n  header_format: 'Authorization: Bearer {access_token}'\n  oauth2_flows: [clientCredentials, authorizationCode]\n  access_token_ttl_seconds: 900\nnotes: >-\n  Every Aspire API request carries an access token as an HTTP bearer token in\n  the Authorization header. Access tokens are short-lived (900 seconds) with no\n  refresh token on the client-credentials flow; request a new token on expiry.\n  An expired or invalid token returns 401 Unauthorized.\nschemes:\n- name: ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Server-to-server access to your own Aspire account. Obtain a Client ID and\n    Client Secret from the Aspire dashboard, then exchange them for an access\n    token via POST https://api.aspireapp.com/public/v1/login.\
  \ Tokens expire in\n    900 seconds; no refresh token is issued.\n  tokenUrl: https://api.aspireapp.com/public/v1/login\n  source: https://docs.api.aspireapp.com/authentication\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  description: >-\n    Third-party apps acting on another user's Aspire data with their consent.\n    Register the app with the Aspire Account Manager to receive a Client ID and\n    Client Secret, redirect the user to the authorization URL, exchange the\n    returned authorization code for an access token plus refresh token, and use\n    the refresh token to mint fresh access tokens.\n  source: https://docs.api.aspireapp.com/authentication\nscopes_summary: >-\n  API keys operate under scopes that limit accessible endpoints (e.g. transfers,\n  quotes). FX transfers require both the transfers and quotes scopes. See\n  scopes/aspire-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspire/refs/heads/main/authentication/aspire-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Fintech
- Business Banking
- Payments
- Payouts
- Card Issuance
- Foreign Exchange
- Expense Management
- Financial Services
- Singapore
---
