---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Opower Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: OPOWER secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: OPOWER
provider_slug: opower
scheme_count: 1
schemes:
- description: 'Oracle Utilities Opower REST APIs use the OAuth 2.0 standard with two-legged authorization: a trusted developer (the utility) obtains an access token using the client_credentials grant and their client_id / client_secret, then passes it as a Bearer token on every request. Tokens are short-lived (expires_in ~3599 seconds).'
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://cxapi.opower.com/apis/authorization-v1/oauth2/token
  guidance: Oracle documents that keys/tokens must not be used directly in a browser or mobile app; utilities must front the Opower APIs with a server-side API gateway that exchanges an end-customer session token for a utility OAuth token.
  name: OAuth2ClientCredentials
  token_request: POST /apis/authorization-v1/oauth2/token with body grant_type=client_credentials, HTTP Basic auth of client_id:client_secret, Content-Type application/x-www-form-urlencoded.
  token_response_fields:
  - client_id
  - access_token
  - token_type
  - expires_in
  type: oauth2
  usage: 'Authorization: Bearer {access_token}'
slug: opower-authentication
source_filename: opower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.oracle.com/en/industries/energy-water/digital-self-service/restapi/UseOAuth.html\ndocs: https://docs.oracle.com/en/industries/energy-water/digital-self-service/restapi/UseOAuth.html\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  model: two-legged (trusted developer / utility) client-credentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  description: >-\n    Oracle Utilities Opower REST APIs use the OAuth 2.0 standard with two-legged\n    authorization: a trusted developer (the utility) obtains an access token using the\n    client_credentials grant and their client_id / client_secret, then passes it as a\n    Bearer token on every request. Tokens are short-lived (expires_in ~3599 seconds).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cxapi.opower.com/apis/authorization-v1/oauth2/token\n    scopes: {}\n  token_request: >-\n    POST /apis/authorization-v1/oauth2/token\
  \ with body grant_type=client_credentials,\n    HTTP Basic auth of client_id:client_secret, Content-Type application/x-www-form-urlencoded.\n  token_response_fields: [client_id, access_token, token_type, expires_in]\n  usage: 'Authorization: Bearer {access_token}'\n  guidance: >-\n    Oracle documents that keys/tokens must not be used directly in a browser or mobile\n    app; utilities must front the Opower APIs with a server-side API gateway that exchanges\n    an end-customer session token for a utility OAuth token.\nscopes: none-documented\nnotes: >-\n  The GraphQL Integration Hub API is likewise OAuth 2.0 secured. No OAuth scopes are\n  documented; access is governed by the utility's provisioned products and roles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opower/refs/heads/main/authentication/opower-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Energy
- Utilities
- Energy Efficiency
- Customer Engagement
- Smart Meter
- Usage Data
- Oracle
---
