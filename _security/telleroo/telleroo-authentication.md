---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Telleroo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Telleroo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Telleroo
provider_slug: telleroo
scheme_count: 2
schemes:
- api: Telleroo Business API
  description: API token generated from the Telleroo dashboard, sent verbatim in the Authorization header (Bearer token). Grants full access to all v1 endpoints; a limited Recipient Access token variant is also available.
  in: header
  name: BusinessAuthorizationToken
  parameter: Authorization
  scheme: bearer
  source: https://docs.telleroo.com/#authentication
  type: http
- api: Telleroo Partner API
  authorizationUrl: https://admin.telleroo.com/oauth
  description: OAuth 2.0 authorization code grant. The partner redirects the client to the Telleroo authorize URL with client_id, redirect_uri, response_type=code and scope=create, then exchanges the returned code for an access token (Bearer, 7200s TTL) and refresh token at the token endpoint.
  flow: authorizationCode
  name: PartnerOAuth2
  refreshUrl: https://api.telleroo.com/oauth/token
  sandbox:
    authorizationUrl: https://sandbox.app.telleroo.com/oauth
    tokenUrl: https://sandbox.telleroo.com/oauth/token
  scopes:
    create: Permission to create pay runs on behalf of a client company
  source: https://partner-docs.telleroo.com/#authentication
  token:
    expires_in: 7200
    refresh_token: supported
    token_type: Bearer
  tokenUrl: https://api.telleroo.com/oauth/token
  type: oauth2
slug: telleroo-authentication
source_filename: telleroo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.telleroo.com/ ; https://partner-docs.telleroo.com/\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Business API (v1) uses a static API token (generated in the Telleroo\n    dashboard) sent in the Authorization request header; all traffic must be\n    over HTTPS. The Partner API (v3) uses OAuth 2.0 authorization code flow to\n    act on behalf of client companies. Two Business token classes exist: a\n    Full Access token (all endpoints, optional auto-approval) and a Recipient\n    Access token (recipient management only, with censored bank details).\nschemes:\n- name: BusinessAuthorizationToken\n  api: Telleroo Business API\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    API token generated from the Telleroo dashboard, sent verbatim in the\n    Authorization header (Bearer token). Grants full\
  \ access to all v1\n    endpoints; a limited Recipient Access token variant is also available.\n  source: https://docs.telleroo.com/#authentication\n- name: PartnerOAuth2\n  api: Telleroo Partner API\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://admin.telleroo.com/oauth\n  tokenUrl: https://api.telleroo.com/oauth/token\n  refreshUrl: https://api.telleroo.com/oauth/token\n  scopes:\n    create: Permission to create pay runs on behalf of a client company\n  token:\n    token_type: Bearer\n    expires_in: 7200\n    refresh_token: supported\n  sandbox:\n    authorizationUrl: https://sandbox.app.telleroo.com/oauth\n    tokenUrl: https://sandbox.telleroo.com/oauth/token\n  description: >-\n    OAuth 2.0 authorization code grant. The partner redirects the client to\n    the Telleroo authorize URL with client_id, redirect_uri, response_type=code\n    and scope=create, then exchanges the returned code for an access token\n    (Bearer, 7200s TTL) and refresh token at the\
  \ token endpoint.\n  source: https://partner-docs.telleroo.com/#authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telleroo/refs/heads/main/authentication/telleroo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Payments
- Bulk Payments
- Payroll
- Faster Payments
- E-Money
- Fintech
- Banking
- International Payments
- Embedded Finance
---
