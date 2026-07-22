---
api_key_in: []
auth_types:
- oauth2
- http
description: 'Raise Commerce API (business/v2) authentication. All requests are authorized with an OAuth 2.0 bearer access token. Two token-issuance flows exist: a server-to-server flow (Tokens resource, HTTP Basic with Client ID + Secret) and an app/web customer flow (Auth resource, with a verification method).'
kind: authentication
layout: security
method: searched
name: Raise Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Raise secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Raise
provider_slug: raise
scheme_count: 2
schemes:
- description: 'Server clients POST to /business/v2/tokens using HTTP Basic auth (Authorization: Basic base64(client_id:client_secret)) to obtain a bearer access token. The token is then sent on all subsequent calls as Authorization: Bearer {access_token}. Tokens issued via /tokens expire in 15 minutes.'
  flow: clientCredentials
  name: serverBearer
  sources:
  - https://docs.raise.com/
  token_expiry: 15 minutes
  token_url: https://commerce-api.raise.com/business/v2/tokens
  type: oauth2
- description: App/Web clients POST to /business/v2/auth/tokens with a customer verification method to obtain a bearer token (valid up to 6 months). Auth methods are registered/updated via POST and PATCH /business/v2/auth/methods and support SR25519 key pair, RSA key pair, SMS one-time code, and TOTP.
  flow: clientCredentials
  name: customerBearer
  sources:
  - https://docs.raise.com/
  token_expiry: 6 months
  token_url: https://commerce-api.raise.com/business/v2/auth/tokens
  type: oauth2
  verification_methods:
  - SR25519 key pair
  - RSA key pair
  - SMS verification code
  - TOTP
slug: raise-authentication
source_filename: raise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.raise.com/\ndocs: https://docs.raise.com/\ndescription: >-\n  Raise Commerce API (business/v2) authentication. All requests are authorized\n  with an OAuth 2.0 bearer access token. Two token-issuance flows exist: a\n  server-to-server flow (Tokens resource, HTTP Basic with Client ID + Secret)\n  and an app/web customer flow (Auth resource, with a verification method).\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: serverBearer\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Server clients POST to /business/v2/tokens using HTTP Basic auth\n    (Authorization: Basic base64(client_id:client_secret)) to obtain a bearer\n    access token. The token is then sent on all subsequent calls as\n    Authorization: Bearer {access_token}. Tokens issued via /tokens expire in\n    15 minutes.\n  token_url: https://commerce-api.raise.com/business/v2/tokens\n\
  \  token_expiry: 15 minutes\n  sources:\n  - https://docs.raise.com/\n- name: customerBearer\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    App/Web clients POST to /business/v2/auth/tokens with a customer\n    verification method to obtain a bearer token (valid up to 6 months). Auth\n    methods are registered/updated via POST and PATCH /business/v2/auth/methods\n    and support SR25519 key pair, RSA key pair, SMS one-time code, and TOTP.\n  token_url: https://commerce-api.raise.com/business/v2/auth/tokens\n  token_expiry: 6 months\n  verification_methods:\n  - SR25519 key pair\n  - RSA key pair\n  - SMS verification code\n  - TOTP\n  sources:\n  - https://docs.raise.com/\nrequired_headers:\n- name: Authorization\n  value: Bearer {access_token}\n- name: Content-Type\n  value: application/json\n- name: X-Country\n  value: ISO 3166-1 alpha-2 country (default US)\n- name: X-Currency\n  value: ISO 4217 currency (default USD)\n- name: X-CustomerID\n  value: customer id (auth\
  \ endpoints)\nnotes: >-\n  Production and sandbox credentials are managed through the Raise Client Portal\n  (portal.raise.com / sandbox-portal.raise.com). A public Playground environment\n  is available without formal onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raise/refs/heads/main/authentication/raise-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Consumer
- Gift Cards
- Commerce
- Payments
- Rewards
- Marketplace
- API
---
