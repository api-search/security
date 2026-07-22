---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tenzo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tenzo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tenzo
provider_slug: tenzo
scheme_count: 1
schemes:
- authorizationUrl: https://auth.gotenzo.com/o/authorize
  flow: authorizationCode
  name: OAuth2
  notes: 'Partner applications are provisioned manually by Tenzo (email partnerships@gotenzo.com) and receive a Client ID, Client Secret, and a granted set of scopes. The Authorization Code grant exchanges an authorization code for an access token (10-hour lifetime) plus a non-expiring refresh token. Access tokens are passed either as an `Authorization: Bearer` header or an `X-AUTH-TOKEN` header on requests to https://api.gotenzo.com/public/v1. HTTPS is required.'
  pkce_supported: true
  redirect_uri_limit: 3
  revocationUrl: https://auth.gotenzo.com/o/revoke_token/
  tokenUrl: https://auth.gotenzo.com/o/token/
  type: oauth2
slug: tenzo-authentication
source_filename: tenzo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.gotenzo.com/developers/auth-flow/\ndocs: https://support.gotenzo.com/developers/auth-flow/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  token_transport:\n  - header: Authorization\n    format: Bearer <access_token>\n  - header: X-AUTH-TOKEN\n    format: <access_token>\n  access_token_lifetime_seconds: 36000\n  refresh_token_expires: false\n  provisioning: manual\n  provisioning_contact: partnerships@gotenzo.com\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  pkce_supported: true\n  authorizationUrl: https://auth.gotenzo.com/o/authorize\n  tokenUrl: https://auth.gotenzo.com/o/token/\n  revocationUrl: https://auth.gotenzo.com/o/revoke_token/\n  redirect_uri_limit: 3\n  notes: >-\n    Partner applications are provisioned manually by Tenzo (email partnerships@gotenzo.com) and\n    receive a Client ID, Client Secret, and a granted set of scopes. The Authorization\
  \ Code grant\n    exchanges an authorization code for an access token (10-hour lifetime) plus a non-expiring\n    refresh token. Access tokens are passed either as an `Authorization: Bearer` header or an\n    `X-AUTH-TOKEN` header on requests to https://api.gotenzo.com/public/v1. HTTPS is required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenzo/refs/heads/main/authentication/tenzo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Restaurant
- Analytics
- Business Intelligence
- Reporting
- Forecasting
- Hospitality
- Point of Sale
- Data Aggregation
- MCP
- Artificial Intelligence
---
